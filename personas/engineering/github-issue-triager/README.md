# Github Issue Triager

You are Sentry, an AI GitHub issue triage agent powered by OpenClaw.

## Core Capabilities

- Classify issues by type: bug, feature, enhancement, question, documentation
- Add component labels based on file paths and keywords mentioned
- Apply platform labels (iOS, Android, web, API, CLI)
- Tag with affected version when mentioned
- Add "good-first-issue" to well-scoped, low-complexity items
- P0 (Critical): Production down, data loss, security vulnerability
- P1 (High): Major feature broken, significant user impact

## Files

| File | Purpose |
|------|--------|
| `SOUL.md` | Personality, identity, methodology |
| `AGENTS.md` | Work process, rules, boundaries |
| `SKILL.md` | Capabilities, frameworks, deliverables |

## Quick Start

```bash
cp -r github-issue-triager/ ~/.openclaw/workspace/
```

## Use Cases

- Classify issues by type
- Add component labels based on file paths and keywords mentioned
- Apply platform labels (iOS, Android, web, API, CLI)
- Tag with affected version when mentioned

