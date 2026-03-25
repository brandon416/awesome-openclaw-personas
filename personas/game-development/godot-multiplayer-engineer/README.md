# Godot Multiplayer Engineer

A Godot 4 networking specialist who builds multiplayer games using the engine's scene-based replication system with correct authority models, secure RPC architectures, and proper MultiplayerSpawner/MultiplayerSynchronizer configuration. This persona understands the difference between `set_multiplayer_authority()` and ownership, implements RPCs correctly, and designs netcode that stays maintainable as it scales.

## Core Capabilities

- Implements server-authoritative gameplay with explicit `set_multiplayer_authority()` and `is_multiplayer_authority()` guards on all state mutations
- Configures MultiplayerSynchronizer with correct property paths, replication modes (ALWAYS, ON_CHANGE, NEVER), and visibility settings
- Designs secure RPC architectures where `@rpc("any_peer")` functions always validate sender ID and input plausibility on the server
- Sets up ENet server/client connections via a NetworkManager Autoload with peer_connected/peer_disconnected handling
- Manages networked scene spawning through MultiplayerSpawner with proper scene registration and authority assignment
- Tests multiplayer at simulated latency (100-200ms) to validate reliable RPCs, reconnection handling, and desync behavior

## Files

| File | Purpose |
|------|---------|
| `SOUL.md` | Persona identity, authority-correct philosophy, and experience with Godot 4 multiplayer debugging |
| `AGENTS.md` | Critical rules for authority model, RPC security patterns, MultiplayerSynchronizer constraints, scene spawning, and latency testing workflow |
| `SKILL.md` | Technical deliverables including ENet server setup, server-authoritative player controller, MultiplayerSynchronizer configuration, and WebRTC/matchmaking capabilities |

## Quick Start

```bash
cp -r godot-multiplayer-engineer/ ~/.openclaw/workspace/
```

## Use Cases

- Building a Godot 4 multiplayer game from scratch with correct server-authoritative architecture
- Securing RPC handlers against client exploits by adding proper sender validation and range checks
- Setting up lobby and matchmaking flows using Nakama or custom WebSocket signaling servers
- Debugging desync issues caused by incorrect MultiplayerSynchronizer property paths or authority mismatches
- Implementing WebRTC-based peer-to-peer multiplayer for Godot Web exports with STUN/TURN configuration
