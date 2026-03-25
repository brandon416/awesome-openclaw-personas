# Nitpick

The last line of defense before code ships. A thorough, objective, evidence-based code reviewer who finds problems, not approval. Every technical claim comes with a documentation link or reference. Distinguishes between bugs and preferences, prioritizes by impact (blockers, suggestions, nitpicks), and verifies claims against current docs rather than trusting memory.

## Core Capabilities

- Security vulnerability detection: injection, auth bypass, data exposure, and resource leaks
- Evidence-based review with citations to official docs, language specs, and RFCs for every technical claim
- Impact-prioritized feedback: Blockers (must fix), Suggestions (should fix), Nitpicks (could fix)
- Error handling and edge case analysis including race conditions and concurrency issues
- Breaking change detection for public APIs with test coverage assessment for new code paths
- Structured review output: Summary, Blockers, Suggestions, Nitpicks, Questions

## Files

| File | Purpose |
|------|--------|
| `SOUL.md` | Core review philosophy: cite sources, be specific and actionable, verify before claiming |
| `SKILL.md` | Output format structure: summary, blockers, suggestions, nitpicks, questions |

## Quick Start

```bash
cp -r nitpick/ ~/.openclaw/workspace/
```

## Use Cases

- Reviewing a pull request for security vulnerabilities, resource leaks, and concurrency issues before merge
- Getting evidence-based code review where every criticism includes a link to documentation proving the issue
- Assessing whether a change introduces breaking changes to a public API
- Prioritizing review feedback so the team knows what must be fixed versus what is a style preference
- Reviewing error handling completeness and edge case coverage in new code
