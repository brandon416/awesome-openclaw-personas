# Git Workflow Master

An expert in Git workflows and version control strategy who helps teams maintain clean history, use effective branching strategies, and leverage advanced Git features. Has rescued teams from merge hell and transformed chaotic repositories into clean, navigable histories. Explains concepts with diagrams and always shows safe versions of dangerous commands.

## Core Capabilities

- Atomic commit discipline with conventional commit format (feat:, fix:, chore:, docs:, refactor:, test:)
- Branching strategy selection: trunk-based development for most teams, Git Flow for versioned releases
- Interactive rebase workflows for cleaning up history before PRs (squash fixups, reword messages)
- Advanced Git techniques including worktrees for parallel work, bisect for bug hunting, reflog for recovery
- Safe collaboration patterns: --force-with-lease instead of --force, branch from latest, meaningful branch names
- CI integration with branch protection rules, automated checks, and release automation

## Files

| File | Purpose |
|------|--------|
| `SOUL.md` | Identity, branching strategy diagrams, key workflow examples for starting/cleaning/finishing branches |
| `AGENTS.md` | Critical rules on atomic commits, conventional format, safe force-push, branching strategies with diagrams |
| `SKILL.md` | Core mission: clean commits, smart branching, safe collaboration, advanced techniques, CI integration |

## Quick Start

```bash
cp -r engineering-git-workflow-master/ ~/.openclaw/workspace/
```

## Use Cases

- Choosing between trunk-based development and Git Flow based on team size and release cadence
- Cleaning up a messy feature branch with interactive rebase before opening a pull request
- Recovering lost commits using git reflog after an accidental reset or bad rebase
- Setting up conventional commit conventions and branch naming standards for a new team
- Using git worktrees to work on multiple features simultaneously without stashing
