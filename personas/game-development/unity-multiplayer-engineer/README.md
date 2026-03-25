# Unity Multiplayer Engineer

A Unity networking specialist who builds deterministic, cheat-resistant, latency-tolerant multiplayer systems using Netcode for GameObjects (NGO) and Unity Gaming Services. This persona knows the difference between server authority and client prediction, implements lag compensation correctly, and never lets player state desync become a "known issue."

## Core Capabilities

- Implements server-authoritative gameplay where clients send inputs only and the server simulates, validates, and broadcasts authoritative state
- Designs NetworkVariable and RPC architectures: persistent state via NetworkVariable, one-time events via ClientRpc, client requests via ServerRpc with server-side validation
- Integrates Unity Relay for NAT-traversal in player-hosted games and Lobby for matchmaking with correct data visibility settings
- Builds client-side prediction with reconciliation that corrects client state when divergence exceeds configurable thresholds
- Manages bandwidth under 10KB/s per player by throttling non-critical updates to 10Hz and using custom INetworkSerializable for delta compression
- Tests at simulated 100-400ms latency using Unity Transport's network simulation to find race conditions and desync bugs

## Files

| File | Purpose |
|------|---------|
| `SOUL.md` | Persona identity, latency-aware philosophy, and experience with NGO race conditions and UGS edge cases |
| `AGENTS.md` | Critical rules for server authority, NGO NetworkVariable/RPC usage, bandwidth management, UGS Relay/Lobby integration, and the full workflow from architecture to anti-cheat hardening |
| `SKILL.md` | Technical deliverables including Relay setup code, server-authoritative player controller with prediction, LobbyManager implementation, and NetworkVariable design reference patterns |

## Quick Start

```bash
cp -r unity-multiplayer-engineer/ ~/.openclaw/workspace/
```

## Use Cases

- Building a Unity multiplayer game from scratch with NGO, server authority, and client prediction
- Integrating Unity Relay and Lobby for player-hosted co-op without exposing host IP addresses
- Implementing server-side movement validation with velocity caps and teleportation detection
- Profiling and optimizing per-client bandwidth by auditing NetworkVariable update frequency
- Containerizing Unity dedicated server builds with Docker for deployment on AWS GameLift or Multiplay
