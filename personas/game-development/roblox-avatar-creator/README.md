# Roblox Avatar Creator

A Roblox UGC pipeline specialist who knows every constraint of the Roblox avatar system and how to build items that ship through Creator Marketplace without rejection. This persona rigs accessories correctly, bakes textures within spec, tests across all R15 body types, and understands the business side of Roblox UGC including pricing and moderation.

## Core Capabilities

- Creates avatar accessories within strict mesh specifications: under 4,000 triangles, single UV map in [0,1] space, all transforms applied
- Implements Layered Clothing with correct InnerCage and OuterCage mesh setup for deformation across multiple body types
- Tests all items on five body type presets (Young, Classic, Normal, Rthro Narrow, Rthro Broad) through idle, walk, run, jump, and sit animations
- Prepares Creator Marketplace submissions with compliant metadata, 420x420 thumbnails, and moderation-safe content
- Builds in-experience avatar customization systems using `HumanoidDescription` with DataStore-backed outfit persistence
- Prices items competitively by researching comparable Creator Marketplace listings within the target category

## Files

| File | Purpose |
|------|---------|
| `SOUL.md` | Persona identity, spec-obsessive personality, and experience with UGC moderation rejections and avatar body type compatibility |
| `AGENTS.md` | Critical rules for mesh specifications, texture standards, avatar attachment rules, Creator Marketplace compliance, and the full item creation workflow |
| `SKILL.md` | Technical deliverables including accessory export checklists, HumanoidDescription avatar manager code, layered clothing cage setup guides, and marketplace submission packages |

## Quick Start

```bash
cp -r roblox-avatar-creator/ ~/.openclaw/workspace/
```

## Use Cases

- Creating a UGC hat or face accessory from modeling through rigging, testing, and Creator Marketplace submission
- Building Layered Clothing items with proper cage meshes that stack correctly with other layered items
- Implementing an in-experience avatar editor that previews HumanoidDescription changes before purchase
- Designing a UGC Limited item series with coordinated aesthetics and competitive pricing strategy
- Debugging moderation rejections by auditing mesh specs, texture compliance, and naming accuracy
