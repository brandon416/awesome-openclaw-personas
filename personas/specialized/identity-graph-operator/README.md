# Identity Graph Operator

Operates a shared identity graph that multiple AI agents resolve against, ensuring every agent in a multi-agent system gets the same canonical answer for "who is this entity?" -- deterministically, even under concurrent writes. Uses evidence-based matching with field-level scoring, nickname normalization, and E.164 phone formatting to resolve records to canonical entities with full audit trails.

## Core Capabilities

- Resolves records to canonical entities using blocking, field-level scoring (email, phone, name with nickname expansion), and configurable confidence thresholds
- Proposes merges with per-field evidence scores rather than executing directly, enabling multi-agent review before mutations commit
- Maintains graph integrity through optimistic locking, mutation simulation (preview without commit), and full event history (created, merged, split, updated)
- Handles real-time resolution in under 100ms via index lookup and batch reconciliation across millions of records with graph clustering
- Supports multi-entity-type graphs (persons, companies, products, transactions) with per-type matching rules and cross-entity relationship discovery
- Enforces tenant isolation with PII masked by default and deterministic resolution where same input always produces same entity_id

## Files

| File | Purpose |
|------|---------|
| `SOUL.md` | Identity resolution schema, merge proposal structure, matching techniques with code examples, cross-framework federation, and integration patterns with other agents |
| `AGENTS.md` | Determinism rules, evidence-over-assertion principles, tenant isolation requirements, workflow steps, and conflict resolution protocol |
| `SKILL.md` | Core mission for record resolution, fuzzy matching capabilities, and canonical entity maintenance |

## Quick Start

```bash
cp -r identity-graph-operator/ ~/.openclaw/workspace/
```

## Use Cases

- Preventing duplicate customer records when multiple agents (billing, support, shipping) encounter the same person from different data sources
- Resolving "Bill Smith" and "William Smith" at the same email to a single canonical entity across a multi-agent CRM system
- Running batch identity reconciliation across millions of records while maintaining consistency with real-time agent lookups
- Building a shared identity layer for agents connecting via MCP, REST API, SDK, or CLI with portable agent identity in audit trails
- Detecting and resolving conflicting merge/split proposals from different agents with evidence-based arbitration
