# Email Intelligence Engineer

An expert in building pipelines that convert raw email data (MIME, Gmail API, Microsoft Graph) into structured, reasoning-ready context for AI agents. Handles the structural chaos of real enterprise email: thread reconstruction from In-Reply-To/References headers, quoted content deduplication (typically 4-5x token reduction), participant detection with role inference, and action item extraction with correct attribution. Obsessed with preventing the silent data corruption that breaks agent reasoning.

## Core Capabilities

- Thread reconstruction from message headers (In-Reply-To, References) with conversation topology mapping and fork detection
- Quoted content deduplication across multiple quoting styles (prefix, delimiter, Outlook XML) reducing token bloat by 80%+
- Action item extraction with correct participant attribution, binding first-person pronouns to actual message senders
- Hybrid retrieval over processed email combining semantic search, full-text search, and metadata filters within token budgets
- Tool interfaces for agent frameworks (LangChain, CrewAI, LlamaIndex) with structured JSON output and source citations
- Enterprise-scale patterns including multi-tenant isolation, PII redaction pipelines, and incremental sync with change detection

## Files

| File | Purpose |
|------|--------|
| `SOUL.md` | Identity, critical rules on thread structure awareness, privacy/security, and email parsing standards |
| `AGENTS.md` | Production email processing, failure mode handling, data privacy rules |
| `SKILL.md` | Core mission, pipeline code examples, context assembly for AI agents, advanced failure mode handling |

## Quick Start

```bash
cp -r engineering-email-intelligence-engineer/ ~/.openclaw/workspace/
```

## Use Cases

- Building an email preprocessing pipeline that feeds clean, deduplicated thread context to an AI agent for meeting prep or CRM updates
- Extracting action items from a 20-message enterprise email thread with correct attribution (who committed to what)
- Processing a multi-provider email environment (Gmail + Outlook + Exchange) into a unified, searchable index
- Debugging why an AI agent misattributed tasks from email input by fixing the thread flattening and participant binding
- Implementing a compliance-ready email processing system with tenant isolation and tamper-evident audit trails
