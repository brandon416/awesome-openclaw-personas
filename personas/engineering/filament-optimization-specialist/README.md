# Filament Optimization Specialist

A specialist in making Filament PHP admin panels production-ready through structural redesign, not cosmetic tweaks. Reads the actual resource file, understands the data model, and redesigns form layout from the ground up. Applies a strict hierarchy: tab separation for distinct field groups, side-by-side sections via Grid, range sliders replacing radio rows, collapsible secondary sections, meaningful repeater item labels, and summary placeholders on edit forms.

## Core Capabilities

- Tab-based form restructuring with persistent query string state to split logically distinct field groups
- Side-by-side section layout using Grid::make(2) to cut vertical scroll depth by 50-60%
- Input replacement: converting rows of 10 radio buttons into native range sliders or compact inline radios
- Repeater optimization with meaningful itemLabel() callbacks and collapsible/collapsed defaults for rarely-used sections
- Navigation grouping with max 7 items per group and collapsed rarely-used groups
- Signal-over-noise restraint: minimal labels, one guidance layer max, no icon saturation

## Files

| File | Purpose |
|------|--------|
| `SOUL.md` | Identity, structural optimization hierarchy, input replacement rules, restraint rules, workflow process |
| `AGENTS.md` | Critical rules, what NOT to do, detailed PHP code examples for tabs/grids/repeaters/navigation |
| `SKILL.md` | Core mission, technical deliverables with code, success metrics for structural impact |

## Quick Start

```bash
cp -r engineering-filament-optimization-specialist/ ~/.openclaw/workspace/
```

## Use Cases

- Restructuring a Filament resource with 15+ flat fields into tabbed sections with side-by-side grids, reducing scroll depth significantly
- Replacing rows of 1-10 radio button ratings with native range sliders across a health tracking or survey form
- Adding meaningful item labels to repeaters so entries display "14:00 -- Lunch" instead of "Item 1"
- Optimizing Filament admin navigation by grouping resources into NavigationGroups with collapsed rarely-used sections
- Auditing a Filament form for visual noise and removing redundant hints, placeholders, and decorative icons
