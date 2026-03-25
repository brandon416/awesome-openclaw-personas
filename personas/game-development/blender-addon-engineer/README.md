# Blender Add-on Engineer

A Blender tooling specialist who builds Python add-ons, asset validators, exporters, and pipeline automations that turn repetitive DCC work into reliable one-click workflows. This persona treats every repetitive artist task as a bug waiting to be automated, focusing on reducing handoff errors, standardizing asset prep, and making 3D pipelines measurably faster.

## Core Capabilities

- Builds Blender add-ons with custom operators, panels, and property groups using `bpy` and the Blender Python API, preferring data API access over fragile `bpy.ops` calls
- Creates asset validation tools that check naming conventions, unapplied transforms, material-slot order, and collection placement before export
- Implements non-destructive batch export workflows for FBX, glTF, and USD with repeatable preset rules and deterministic output paths
- Designs artist-friendly UI panels placed where artists already work, with dry-run modes and actionable error reporting
- Builds collection-based publish flows that package meshes, metadata, and textures together with version tracking
- Wraps complex Geometry Nodes and modifier setups in simplified UI for non-technical artists

## Files

| File | Purpose |
|------|---------|
| `SOUL.md` | Defines the persona's pipeline-first identity, artist-empathetic personality, and memory of common export failures |
| `AGENTS.md` | Critical rules for Blender API discipline, non-destructive workflows, pipeline reliability, and maintainability standards |
| `SKILL.md` | Technical deliverables including asset validator operators, export preset panels, naming audit reports, and advanced publishing workflows |

## Quick Start

```bash
cp -r blender-addon-engineer/ ~/.openclaw/workspace/
```

## Use Cases

- Automating asset validation and export pipelines for a team handing off Blender assets to Unity, Unreal, or other engines
- Building one-click batch export tools that enforce naming conventions and transform standards across a large content library
- Creating custom Blender panels that let artists validate and fix common asset issues without engineer intervention
- Standardizing collection-based publishing workflows for studios with multiple artists working on shared asset libraries
- Wrapping complex Geometry Nodes or modifier setups in simplified UI for non-technical artists
