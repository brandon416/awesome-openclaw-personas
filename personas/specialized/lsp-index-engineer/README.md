# LSP/Index Engineer

Specialized systems engineer who orchestrates multiple Language Server Protocol clients and builds unified code intelligence systems. Transforms heterogeneous language servers (TypeScript, PHP, Go, Rust, Python) into a cohesive semantic graph that powers real-time code visualization with sub-100ms response times and WebSocket-streamed graph diffs.

## Core Capabilities

- Builds the graphd LSP aggregator that orchestrates concurrent LSP clients across multiple languages with proper capability negotiation per LSP 3.17
- Transforms LSP responses into a unified graph schema with file nodes, symbol nodes, and typed edges (contains, imports, extends, implements, calls, references)
- Implements real-time incremental graph updates via file watchers and git hooks with atomic updates that never leave the graph inconsistent
- Creates nav.index.jsonl with symbol definitions, references, and hover documentation, plus LSIF import/export for pre-computed semantic data
- Maintains performance contracts: /graph endpoint under 100ms for 10k nodes, /nav/:symId lookups under 20ms cached, WebSocket latency under 50ms
- Applies advanced graph algorithms (Tarjan's SCC, PageRank for importance) with lock-free data structures and SIMD optimizations

## Files

| File | Purpose |
|------|---------|
| `SOUL.md` | LSP/Index Engineer identity, multi-language LSP experience, and protocol-focused personality |
| `AGENTS.md` | LSP protocol compliance rules, graph consistency requirements, performance contracts, workflow steps, and pattern recognition expertise |
| `SKILL.md` | graphd core architecture (TypeScript interfaces), LSP client orchestration code, graph construction pipeline, navigation index format, and advanced capabilities |

## Quick Start

```bash
cp -r lsp-index-engineer/ ~/.openclaw/workspace/
```

## Use Cases

- Building a unified code intelligence backend for an IDE that supports TypeScript, PHP, Go, Rust, and Python in the same workspace
- Creating a real-time semantic code graph that streams diffs via WebSocket to a visualization frontend at 60fps
- Implementing go-to-definition and hover documentation across a polyglot monorepo with sub-150ms response times
- Pre-computing semantic data with LSIF for large codebases where real-time LSP requests would be too slow
- Optimizing graph queries for 100k+ symbols with progressive loading, lazy evaluation, and memory-mapped files
