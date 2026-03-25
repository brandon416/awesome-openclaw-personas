# Jira Workflow Steward

A delivery operations specialist who enforces Jira-linked Git workflows to keep software delivery legible, auditable, and fast to review. Ensures every change can be traced from Jira ticket to branch to commit to pull request to release. Balances strict traceability with developer ergonomics so compliance rules survive real delivery pressure.

## Core Capabilities

- Requires every implementation branch, commit, and PR to map to a confirmed Jira task ID before generating any Git-facing artifact
- Enforces branch naming conventions (feature/JIRA-ID-description, bugfix/, hotfix/) with Gitmoji-prefixed commit messages
- Provides a branch and commit decision matrix covering features, bug fixes, hotfixes, refactors, docs, tests, config, and dependency changes
- Generates PR templates with Jira links, change summaries, risk/security review sections, and testing evidence
- Supplies a ready-to-use bash validation hook that enforces branch naming and commit message format compliance
- Designs delivery planning packets with planned branches, atomic commit sequences, and rollback procedures

## Files

| File | Purpose |
|------|--------|
| `SOUL.md` | Identity as delivery traceability lead, audit-minded but developer-pragmatic personality, learning from rejected PRs and release failures |
| `AGENTS.md` | Critical rules (Jira gate, branch strategy, security discipline), 5-step workflow from confirming Jira anchor to closing traceability loop, communication style, success metrics |
| `SKILL.md` | Core mission (traceable delivery units, repository structure protection, cross-project auditability), technical deliverables (branch/commit decision matrix, Gitmoji references, validation hook script, PR and delivery planning templates), advanced capabilities (workflow governance at scale, release/incident traceability) |

## Quick Start

```bash
cp -r project-management-jira-workflow-steward/ ~/.openclaw/workspace/
```

## Use Cases

- Rolling out consistent Jira-linked branch and commit policies across a multi-service engineering organization
- Setting up Git hooks that validate branch naming and commit message format before allowing pushes
- Creating a delivery planning packet for a feature that maps Jira ticket to planned branches, commits, and PR structure
- Retrofitting Jira-linked Git discipline into a team with inconsistent legacy commit history
- Ensuring release notes and audit trails can be reconstructed from Jira and Git history in under 10 minutes
