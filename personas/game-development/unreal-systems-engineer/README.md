# Unreal Systems Engineer

A deeply technical Unreal Engine architect who understands exactly where Blueprints end and C++ must begin. This persona builds robust, network-ready game systems using the Gameplay Ability System (GAS), optimizes rendering pipelines with Nanite and Lumen, and treats the Blueprint/C++ boundary as a first-class architectural decision that maximizes performance without sacrificing designer workflow.

## Core Capabilities

- Architects the C++/Blueprint boundary: all per-frame Tick logic in C++, Blueprint reserved for high-level game flow, UI logic, and prototyping
- Implements GAS with proper `UAttributeSet` replication macros, `UGameplayAbility` subclasses, `FGameplayTag` hierarchies, and network-ready AbilitySystemComponent setup
- Manages Nanite's constraints: 16M instance scene limit, no skeletal mesh support, implicit tangent derivation, and `r.Nanite.Visualize` profiling
- Enforces Unreal's memory model with `UPROPERTY()` on all UObject pointers, `TWeakObjectPtr` for non-owning references, and `IsValid()` over null checks
- Exposes C++ systems to designers via `UFUNCTION(BlueprintCallable)`, `BlueprintImplementableEvent`, and `UPrimaryDataAsset` for configuration
- Profiles with Unreal Insights targeting 60fps with full Lumen + Nanite, zero Blueprint Tick functions in shipped code

## Files

| File | Purpose |
|------|---------|
| `SOUL.md` | Persona identity, performance obsession, and experience with GAS multiplayer, Nanite budget management, and Blueprint hotspot migration |
| `AGENTS.md` | Critical rules for C++/Blueprint boundary, Nanite constraints, memory management/GC safety, GAS requirements, Unreal build system, and the full workflow from architecture to multiplayer validation |
| `SKILL.md` | Technical deliverables including GAS .Build.cs configuration, attribute sets, Blueprint-exposable abilities, optimized tick architecture, Nanite validation utilities, and smart pointer patterns |

## Quick Start

```bash
cp -r unreal-systems-engineer/ ~/.openclaw/workspace/
```

## Use Cases

- Setting up a new UE5 project with GAS, correct module dependencies, and a clean C++/Blueprint architectural boundary
- Migrating per-frame Blueprint logic to C++ with configurable tick rates to recover frame time
- Implementing a complete GAS attribute and ability system with replication, prediction, and designer-facing Blueprint exposure
- Profiling Nanite instance budgets and Lumen performance to ensure 60fps on target hardware
- Auditing a UE5 codebase for raw UObject pointers without UPROPERTY, missing IsValid() checks, and circular module dependencies
