# Planner

The central orchestrator of the OpenClaw multi-agent academic system, combining project manager, research advisor, and operations director roles. Decomposes high-level research goals into phased execution plans, coordinates all sub-agents (including custom agents), manages deadline-driven schedules, and enforces quality gates including the Critic's SHARP taste checkpoints.

## Core Capabilities

- Decomposes research objectives into 9 phases (trend sensing through final review) with explicit agent assignments, deliverables, and Critic taste gates at each checkpoint
- Manages DDL-driven reverse planning with Gantt-style timelines, tracking parallel tasks, dependencies, and bottlenecks across agents
- Coordinates conflict resolution between agents (Ideator vs Critic, Writer vs Reviewer) with a 3-round escalation protocol to the main agent
- Enforces quality gates: SHARP >= 18 for idea approval, Parsimony >= 4 for method design, memorability check for drafts, and Critic sign-off before submission
- Manages custom agent lifecycle: evaluates necessity, integrates into workflows, and reviews retention after project completion
- Generates structured status updates with completion tracking, risk flags, and agent health monitoring

## Files

| File | Purpose |
|------|--------|
| `SOUL.md` | Orchestrator identity, task decomposition methodology, DDL management, decision principles, output templates |
| `AGENTS.md` | Model config, persistent project state board, SHARP cross-referencing, escalation protocol |
| `USER.md` | Research domain (AI/NLP/Multi-Agent), Gantt-style communication preference, high DDL sensitivity |

## Quick Start

```bash
cp -r academic-planner/ ~/.openclaw/workspace/
```

## Use Cases

- Create a phased research plan working backwards from a conference submission deadline with agent assignments and milestones
- Coordinate a multi-agent workflow where the Ideator, Critic, Coder, and Writer must hand off work in sequence with quality checkpoints
- Resolve a deadlock between the Ideator and Critic when an idea fails SHARP evaluation after multiple revision rounds
- Generate a weekly status report showing phase progress, blocked tasks, and risk items for a research project
- Evaluate whether a new custom agent is needed for a specialized task or whether existing agents can cover the requirement
