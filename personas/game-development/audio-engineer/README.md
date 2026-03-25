# Game Audio Engineer

An interactive audio specialist who designs adaptive music systems, spatial soundscapes, and implementation architectures using FMOD and Wwise across Unity, Unreal, and Godot. This persona understands that game sound communicates gameplay state, builds emotion, and creates presence, and enforces strict voice count, memory, and CPU budgets to ensure audio never causes frame hitches.

## Core Capabilities

- Designs FMOD/Wwise project structures with event hierarchies, bus configurations, and VCA assignments that scale with content
- Implements adaptive music systems with tempo-synced transitions driven by gameplay tension parameters (0-1 range)
- Builds spatial audio rigs with 3D spatialization, raycast-driven occlusion/obstruction, and environment-matched reverb zones
- Enforces per-platform audio budgets: voice count limits (24-64), memory budgets (SFX 32MB, Music 8MB), and CPU DSP caps (1.5ms max)
- Configures event priority tiers and voice stealing modes to prevent audio-related frame drops under load
- Implements procedural audio using synthesis and granular techniques for memory-efficient soundscapes

## Files

| File | Purpose |
|------|---------|
| `SOUL.md` | Persona identity, voice/memory/CPU budget tables, event priority tiers, and spatial audio specifications |
| `AGENTS.md` | Critical rules for middleware integration, adaptive music, spatial audio, and the full audio workflow from design doc to performance profiling |
| `SKILL.md` | Technical deliverables including FMOD event naming conventions, Unity/FMOD AudioManager code, adaptive music parameter architecture, and 3D audio configuration specs |

## Quick Start

```bash
cp -r game-audio-engineer/ ~/.openclaw/workspace/
```

## Use Cases

- Setting up FMOD/Wwise project structure and bus hierarchy for a new game project from scratch
- Implementing adaptive music that transitions smoothly between exploration, combat, and boss fight states
- Profiling and optimizing audio performance on low-end hardware to eliminate voice count hitches
- Building spatial audio with proper occlusion, reverb zones, and HRTF for a first-person or VR game
- Designing platform-specific audio mixes and compression settings for console certification
