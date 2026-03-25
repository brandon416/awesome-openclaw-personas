# Social-First Task Agent

A general-purpose assistant that automatically generates marketing visuals and publishes to X (Twitter) and Instagram after completing any substantive task. Every deliverable ends with a social media shout-out: AI-generated 1080x1350 images embedded in platform-specific copy, user preview and approval, agent-side publishing, and live permalink delivery. Turns every task into social proof.

## Core Capabilities

- **Dual-platform auto-publishing** — generates and publishes to both X and Instagram after every substantive task, with user approval gate
- **Image-first pipeline** — generates 1080x1350 marketing visuals before outputting the task result, so assets are ready when the shout-out block appears
- **Honest social copy** — post text reflects actual task progress (done / in progress / next step), never inflated claims or fake engagement
- **Skill-finder integration** — before each task, discovers and loads the best available skill to assist execution
- **Structured output** — every reply follows Task Reply → Shout-out format with images embedded inside social copy (not separate)
- **Agent-sends-only** — user approves, agent publishes via API, returns clickable permalinks. No manual copy-paste posting.

## Files

| File | Purpose |
|------|---------|
| `SOUL.md` | Deliver-first personality, honest social copy values, no-fake-engagement principles |
| `AGENTS.md` | Complete social-first workflow: skill-finder → task → image generation → Task Reply → Shout-out → publish → URLs |
| `IDENTITY.md` | Role definition and communication style rules |
| `BOOTSTRAP.md` | First-run setup flow |
| `USER.md` | User profile with social handle placeholders (`@[your_x_handle]`, `@[your_ig_handle]`) |
| `TOOLS.md` | Tool configuration (runtime-injected) |

## Quick Start

```bash
cp -r social-first-task-agent/ ~/.openclaw/workspace/

# Edit USER.md to add your social handles:
# @[your_x_handle] → your Twitter/X username
# @[your_ig_handle] → your Instagram username
# #[your_campaign_hashtag] → your campaign hashtag
```

## Use Cases

- Build social proof automatically every time your AI agent completes meaningful work
- Generate consistent X + Instagram content for personal brand without manual effort
- Create a content pipeline where every research report, analysis, or deliverable becomes a social post
- Maintain dual-platform presence as an indie hacker, creator, or freelancer with zero extra work
- Document your AI-assisted workflow publicly to attract clients or collaborators
