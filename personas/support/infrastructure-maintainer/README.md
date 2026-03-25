# Infrastructure Maintainer

Expert infrastructure specialist who ensures system reliability, performance, and security across all technical operations. Maintains 99.9%+ uptime through Prometheus/Grafana monitoring with predictive alerting, manages Infrastructure as Code with Terraform, implements automated encrypted backup/recovery systems with S3 offsite storage, and optimizes costs through right-sizing and auto-scaling -- all while maintaining SOC2/ISO27001 compliance.

## Core Capabilities

- Maintains 99.9%+ system uptime with comprehensive Prometheus monitoring, Grafana dashboards, and alert rules for CPU (>80%), memory (>90%), disk (>85%), and service availability
- Deploys Infrastructure as Code with Terraform including VPC networking, auto-scaling groups, RDS databases with encryption, and performance insights monitoring
- Implements automated backup and recovery with encrypted (AES256/GPG) database dumps and file archives, S3 offsite storage, integrity verification, and 30-day retention management
- Optimizes infrastructure costs through resource right-sizing, reserved capacity analysis, auto-scaling policies, and spending dashboards with optimization recommendations
- Enforces security through vulnerability management, patch automation, least-privilege access control, multi-factor authentication, and incident response procedures
- Produces infrastructure health reports covering uptime metrics, MTTR, cost per user, security posture, and capacity planning with growth projections

## Files

| File | Purpose |
|------|---------|
| `SOUL.md` | Infrastructure maintainer identity, proactive personality, experience with systems failing from poor monitoring and succeeding with proactive maintenance |
| `AGENTS.md` | Reliability-first rules, security and compliance integration requirements, Prometheus alert rules (CPU, memory, disk, service down), four-step workflow, and success metrics |
| `SKILL.md` | Prometheus monitoring configuration, Terraform AWS infrastructure (VPC, subnets, auto-scaling, RDS), automated backup/recovery bash script with encryption and S3 upload, and advanced capabilities for multi-cloud, Kubernetes, and observability |

## Quick Start

```bash
cp -r support-infrastructure-maintainer/ ~/.openclaw/workspace/
```

## Use Cases

- Setting up Prometheus monitoring with Grafana dashboards and alert rules that detect high CPU, memory exhaustion, and service outages before they impact users
- Deploying a complete AWS infrastructure with Terraform: VPC, private/public subnets, auto-scaling groups, and encrypted RDS databases with automated backups
- Implementing an automated backup system that encrypts database dumps and file archives, uploads to S3, verifies integrity, and manages retention with Slack notifications
- Conducting a cost optimization review that identifies right-sizing opportunities, recommends reserved capacity, and projects 20%+ annual infrastructure savings
- Performing a security audit covering vulnerability assessment, patch management status, access control review, and SOC2 compliance readiness
