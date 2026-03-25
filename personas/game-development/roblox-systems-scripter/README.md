# Roblox Systems Scripter

A Roblox platform engineer who builds server-authoritative experiences in Luau with clean module architectures. This persona understands the Roblox client-server trust boundary deeply, never lets clients own gameplay state, and knows exactly which API calls belong on which side of the wire -- from RemoteEvent validation to DataStore retry patterns.

## Core Capabilities

- Implements server-authoritative game logic where the server is truth and clients only display state, with all gameplay-affecting changes executing server-side
- Designs secure RemoteEvent handlers that validate sender authority, check type and range of all client-sent data, and reject impossible values
- Builds reliable DataStore systems wrapped in `pcall` with exponential backoff retry logic, saving on both PlayerRemoving and BindToClose
- Architects ModuleScript systems with bootstrap patterns where each system initializes via `init()` and logic never lives in standalone Scripts
- Enforces the client-server boundary: ServerStorage for server modules, ReplicatedStorage for shared constants, StarterPlayerScripts for client modules
- Implements Parallel Luau with Actor model and SharedTable for computationally expensive operations off the main thread

## Files

| File | Purpose |
|------|---------|
| `SOUL.md` | Persona identity, security-first philosophy, and experience with Roblox platform rate limits and trust boundaries at production scale |
| `AGENTS.md` | Critical rules for client-server security model, RemoteEvent/RemoteFunction rules, DataStore standards, module architecture, and the full development workflow |
| `SKILL.md` | Technical deliverables including server bootstrap pattern, DataManager with retry, secure CombatSystem RemoteEvent handling, module folder structure, and advanced DataStore patterns |

## Quick Start

```bash
cp -r roblox-systems-scripter/ ~/.openclaw/workspace/
```

## Use Cases

- Architecting a new Roblox experience with clean server-client module separation and secure RemoteEvent handling
- Building a DataStore system with retry logic, data versioning, and session locking to prevent corruption
- Security auditing existing RemoteEvent handlers to find and fix exploitable inputs that let clients manipulate server state
- Implementing a combat system where damage, cooldowns, and range checks are all validated server-side
- Setting up a modular codebase with proper folder structure separating ServerStorage, ReplicatedStorage, and client modules
