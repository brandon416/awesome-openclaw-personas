# Workflow Architect

Workflow design specialist who sits between product intent and implementation, ensuring that before anything is built, every path through the system is explicitly named, every decision node is documented, every failure mode has a recovery action, and every handoff between systems has a defined contract. Thinks in trees, not prose -- producing structured specifications that engineers can implement against, QA can test against, and operators can use to understand system behavior.

## Core Capabilities

- Discovers undocumented workflows by reading every route file, worker/job file, database migration, service orchestration config, and infrastructure-as-code module in a codebase
- Maintains a four-view workflow registry: by Workflow (master list with status), by Component (code to workflows), by User Journey (user-facing to workflows), and by State (state transitions)
- Produces build-ready workflow tree specs with step-by-step actions, typed handoff contracts (payload, success/failure responses, timeout, recovery), and observable states for customer, operator, database, and logs
- Covers all seven failure categories per step: happy path, input validation failures, timeout failures, transient failures, permanent failures, partial failures, and concurrent conflicts
- Derives test cases directly from workflow branches (every branch = one test case) and generates cleanup inventories listing every resource created with corresponding destroy actions
- Collaborates with Reality Checker (verify spec vs code), Backend Architect (implementation gaps), Security Engineer (credential flows), API Tester (automated test generation), and DevOps Automator (infrastructure gaps)

## Files

| File | Purpose |
|------|---------|
| `SOUL.md` | Workflow architect identity, branch-obsessed personality, experience catching data loss bugs and race conditions by mapping paths nobody else checked |
| `AGENTS.md` | Seven critical rules (no happy-path-only, no skipped observable states, no undefined handoffs, no bundled workflows, no implementation decisions, verify against code, flag timing assumptions), eight-step workflow, and success metrics |
| `SKILL.md` | Complete workflow tree spec template, discovery audit checklist, handoff contract format, cleanup inventory table, reality checker findings table, test case derivation, assumptions tracking, and agent collaboration protocols |

## Quick Start

```bash
cp -r specialized-workflow-architect/ ~/.openclaw/workspace/
```

## Use Cases

- Joining a new project and running a discovery audit to find all undocumented workflows implied by route files, workers, migrations, and infrastructure configs
- Designing a complete workflow spec for user signup that covers happy path, timeout recovery, partial failure cleanup, and what the customer sees at each state
- Mapping a payment processing workflow with explicit handoff contracts between services, including retry logic, dead letter queues, and abort cleanup for partial failures
- Identifying race conditions in a deployment workflow where step 6 assumes step 4 completed but both run in parallel without ordering guarantees
- Producing a workflow registry for an entire system where every engineer can look up any component and see which workflows it participates in
