# Agents Orchestrator

Autonomous pipeline manager that orchestrates the entire development workflow from specification to production-ready implementation. Coordinates multiple specialist agents through a PM, Architecture, Dev-QA loop, and Integration pipeline, enforcing quality gates at every stage with automatic retry logic and evidence-based validation.

## Core Capabilities

- Runs a full four-phase pipeline autonomously: Project Manager creates task list, ArchitectUX builds foundation, Developer-QA loops validate task-by-task, and Reality Checker performs final integration testing
- Enforces task-by-task quality gates where each implementation must pass EvidenceQA with screenshot proof before advancing to the next task
- Implements automatic retry logic with maximum 3 attempts per task, passing specific QA feedback back to developers on each loop
- Coordinates 40+ specialist agents across design, engineering, marketing, product management, support, and testing domains
- Produces structured status reports tracking pipeline progress, QA cycles, retry counts, and completion predictions
- Handles agent spawn failures, task implementation failures, and QA validation failures with documented escalation procedures

## Files

| File | Purpose |
|------|---------|
| `SOUL.md` | Pipeline identity, workflow phases, error handling procedures, status reporting templates, and completion summary format |
| `AGENTS.md` | Quality gate enforcement rules, pipeline state management, Dev-QA loop decision logic, and communication style |
| `SKILL.md` | Four-phase orchestration methodology, specialist agent catalog (40+ agents), intelligent retry logic, and context-aware agent spawning |

## Quick Start

```bash
cp -r agents-orchestrator/ ~/.openclaw/workspace/
```

## Use Cases

- Running an end-to-end development pipeline for a new web application from a single project specification file
- Coordinating frontend, backend, and mobile developer agents with automated QA validation after each task
- Managing a multi-agent project where quality gates prevent broken functionality from advancing through the pipeline
- Automating the development workflow for teams that need predictable, evidence-based delivery with screenshot proof at every stage
- Orchestrating large projects where 8+ tasks need sequential Dev-QA loops with failure tracking and escalation
