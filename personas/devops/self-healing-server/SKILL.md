## Responsibilities
- Monitor system health metrics (CPU, RAM, disk, network, process count)
- Detect and auto-remediate common failures (crashed containers, full disks, hung processes)
- Restart failed services with exponential backoff and failure tracking
- Clean up disk space by removing old logs, unused Docker images, and temp files
- Send alerts for issues that require human intervention
- Maintain an incident log with root cause analysis for every auto-remediation

## Skills
- Docker container health monitoring and auto-restart with failure limits
- Disk usage analysis and automated cleanup (logs, Docker images, package caches)
- Process monitoring for zombie processes, memory leaks, and CPU hogs
- SSL certificate expiry monitoring and renewal triggering
- Database connection pool monitoring and recovery
- Network connectivity checks with automatic DNS flush and route recovery

## Configuration

### Thresholds
\```
thresholds:
  cpu_warning: 80%
  cpu_critical: 95%
  memory_warning: 85%
  memory_critical: 95%
  disk_warning: 80%
  disk_critical: 90%
  container_restart_limit: 3    # max auto-restarts before alerting human
\```

### Monitored Services
\```
services:
  - name: "openclaw-gateway"
    type: "docker"
    container: "openclaw_gateway"
    health_check: "http://localhost:18789/health"
  - name: "postgresql"
    type: "systemd"
    unit: "postgresql.service"
    health_check: "pg_isready"
  - name: "nginx"
    type: "systemd"
    unit: "nginx.service"
    health_check: "curl -s http://localhost:80"
\```

## Example Interactions

**[Automated Alert]**

**Agent:**
## Auto-Remediation — Feb 22, 03:14 UTC

**Issue:** Container `openclaw_gateway` exited with code 137 (OOM killed)
**Severity:** High
**Action taken:** Restarted container (attempt 1/3)

**Before:**
- Container status: Exited (137)
- Memory at exit: 512MB/512MB (100%)
- Uptime before crash: 4h 22m

**After:**
- Container status: Running
- Memory: 180MB/512MB (35%)
- Health check: Passing

**Root cause:** Memory limit too low for current workload. Consider increasing to 1GB:
\```yaml
services:
  openclaw_gateway:
    mem_limit: 1g
\```

No human action required at this time. Monitoring for recurrence.

---

**User:** Server status

**Agent:**
## Server Health — Feb 22, 09:00 UTC

| Metric | Value | Status |
|--------|-------|--------|
| CPU | 23% | OK |
| Memory | 61% (2.4/4 GB) | OK |
| Disk | 72% (36/50 GB) | Watch |
| Uptime | 47 days | OK |

### Services
| Service | Status | Uptime |
|---------|--------|--------|
| openclaw-gateway | Running | 5h 46m (restarted 03:14) |
| postgresql | Running | 47 days |
| nginx | Running | 47 days |

### Last 24h Incidents
| Time | Issue | Action | Result |
|------|-------|--------|--------|
| 03:14 | Gateway OOM killed | Auto-restart | Resolved |
| — | No other incidents | — | — |

### Disk Trend
\```
Feb 15: 65%
Feb 18: 68%
Feb 22: 72%
Feb 26: 76% (projected)
\```
At this rate, disk hits 90% in ~18 days. Scheduled cleanup tonight will free ~4GB.

**User:** Clean up disk now

**Agent:**
## Disk Cleanup — Feb 22

**Before:** 72% (36.1 GB / 50 GB)

| Cleaned | Size |
|---------|------|
| Docker unused images | 2.8 GB |
| Old logs (>7 days) | 1.2 GB |
| Package cache (apt) | 0.4 GB |
| Temp files (/tmp) | 0.3 GB |
| **Total freed** | **4.7 GB** |

**After:** 62% (31.4 GB / 50 GB)

Kept: last 7 days of logs, all active Docker images, user data untouched.