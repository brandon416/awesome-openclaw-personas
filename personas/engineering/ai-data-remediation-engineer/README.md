# AI Data Remediation Engineer

A surgical specialist for fixing broken data at scale using air-gapped local SLMs and semantic clustering. Does not rebuild pipelines or redesign schemas. Instead, it intercepts anomalous data, compresses millions of errors into dozens of semantic clusters, generates deterministic fix logic via Ollama (Phi-3, Llama-3, Mistral), and guarantees zero data loss with mathematical reconciliation checks. PII never leaves the local perimeter.

## Core Capabilities

- Semantic anomaly compression using local sentence-transformers and ChromaDB/FAISS to reduce millions of broken rows into 8-15 pattern clusters
- Air-gapped SLM fix generation via Ollama producing sandboxed Python lambdas, with strict validation rejecting any unsafe code
- Zero-data-loss guarantee enforced by mathematical reconciliation: Source == Success + Quarantine on every batch
- PII protection with zero network egress from the remediation layer -- all embeddings and inference run locally
- Hybrid fingerprinting combining SHA-256 primary key hashing with vector similarity to prevent false-positive merges
- Full audit trail logging every row change with old value, new value, lambda applied, confidence score, model version, and timestamp

## Files

| File | Purpose |
|------|--------|
| `SOUL.md` | Identity, critical safety rules (AI generates logic not data, PII perimeter, lambda validation), workflow steps with code |
| `AGENTS.md` | Critical rules on lambda safety gates, PII isolation, hybrid fingerprinting, and audit requirements |
| `SKILL.md` | Core mission: semantic compression, air-gapped SLM fix generation, zero-data-loss guarantees |

## Quick Start

```bash
cp -r engineering-ai-data-remediation-engineer/ ~/.openclaw/workspace/
```

## Use Cases

- Fixing 50,000+ date format errors in a data pipeline by clustering them into ~12 patterns and generating targeted lambda fixes
- Remediating broken data containing PII (SSNs, medical records) where no cloud API can be used
- Building a self-healing remediation layer that sits between validation and staging in an existing data pipeline
- Auditing every AI-applied data transformation with a complete, queryable log for compliance requirements
- Routing low-confidence fixes (below 0.75) to a human quarantine dashboard while auto-fixing high-confidence patterns
