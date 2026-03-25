# Salesforce Architect

Senior Salesforce Solution Architect with deep expertise in multi-cloud platform design (Sales, Service, Marketing, Commerce, Data Cloud, Agentforce), enterprise integration patterns, governor limit-aware application design, and technical governance. Combines strategic roadmap thinking with hands-on Apex, LWC, and data modeling execution to turn tangled orgs into architectures that scale.

## Core Capabilities

- Designs governor limit-aware applications with explicit SOQL (100), DML (150), CPU (10s sync/60s async), and heap (6MB/12MB) budget tracking per transaction
- Selects integration patterns per external system (Platform Events for business events, CDC for data sync, MuleSoft middleware with retry/circuit breaker/DLQ) with ASCII architecture diagrams
- Enforces data model governance: master-detail vs. lookup decisions documented, sharing model designed (OWD + rules), large data volume strategy, and external ID fields for integrations
- Produces Architecture Decision Records (ADRs) with alternatives considered, governor limit impact per option, and scheduled review dates
- Implements Apex patterns (trigger framework with one trigger per object, selector-service-domain layers), LWC patterns (wire adapters, event communication), and Flow bulkification
- Covers Agentforce architecture: agents within governor limits, version-controlled prompt templates, Data Cloud RAG grounding, and Einstein Trust Layer guardrails

## Files

| File | Purpose |
|------|---------|
| `SOUL.md` | Salesforce architect identity, pattern memory for recurring architectural decisions and org-specific constraints, experience with 200-object orgs |
| `AGENTS.md` | Seven critical rules (governor limits non-negotiable, bulkification mandatory, no business logic in triggers, declarative first), four-step workflow, and communication style |
| `SKILL.md` | Multi-cloud architecture domains, ADR template, integration pattern diagram, data model review checklist, governor limit budget tracker, Platform Events vs CDC comparison, and Agentforce architecture guidance |

## Quick Start

```bash
cp -r specialized-salesforce-architect/ ~/.openclaw/workspace/
```

## Use Cases

- Assessing a Salesforce org with technical debt (47 competing flows, hard-coded triggers) and producing a remediation roadmap with governor limit headroom analysis
- Designing a multi-cloud architecture spanning Sales Cloud, Service Cloud, and Data Cloud with single-source-of-truth ownership per data domain
- Selecting between Platform Events and Change Data Capture for a real-time integration with an external ERP system
- Building a deployment pipeline with Salesforce DX, scratch orgs, and CI/CD that supports daily releases without manual changeset management
- Architecting Agentforce agents that operate within governor limits using Data Cloud retrieval for RAG patterns and version-controlled prompt templates
