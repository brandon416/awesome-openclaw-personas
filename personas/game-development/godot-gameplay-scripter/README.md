# Godot Gameplay Scripter

A Godot 4 specialist who builds gameplay systems with strict type safety, signal-driven architecture, and clean node composition using GDScript 2.0 and C#. This persona enforces the "everything is a node" philosophy, treats signals as public APIs with typed parameters, and knows exactly where GDScript ends and C# must begin for performance or library access.

## Core Capabilities

- Enforces mandatory static typing in GDScript 2.0 with zero untyped `var` declarations, typed arrays, and `@export` with explicit types
- Designs signal architectures with typed parameters following language-specific conventions (snake_case for GDScript, PascalCase with EventHandler for C#)
- Implements composition-based character systems using HealthComponent, MovementComponent, and other self-contained node components
- Manages cross-scene communication through a Signal Bus Autoload pattern while keeping Autoloads restricted to genuine global state
- Bridges GDScript and C# interop correctly, including cross-language signal connections and type conversions
- Builds Resource-based data definitions (ScriptableObject equivalent) for designer-facing configuration

## Files

| File | Purpose |
|------|---------|
| `SOUL.md` | Persona identity, composition-first philosophy, and experience with Godot 4 node-tree anti-patterns |
| `AGENTS.md` | Critical rules for signal naming, static typing, node composition, Autoload hygiene, scene lifecycle, and full code examples for each pattern |
| `SKILL.md` | Technical deliverables including typed signal declarations, EventBus Autoload, composition-based player controller, resource data patterns, and GDExtension integration |

## Quick Start

```bash
cp -r godot-gameplay-scripter/ ~/.openclaw/workspace/
```

## Use Cases

- Architecting a new Godot 4 project with clean composition patterns and type-safe signal wiring from the start
- Refactoring monolithic character scripts into single-responsibility component nodes that communicate via signals
- Setting up GDScript/C# interop for a project that needs .NET library access alongside GDScript gameplay code
- Designing an EventBus Autoload for cross-scene communication without creating global state nightmares
- Auditing an existing Godot project to eliminate untyped variables, direct parent references, and broken signal connections
