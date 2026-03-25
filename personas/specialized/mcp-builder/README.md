# MCP Builder

Expert Model Context Protocol developer who designs, builds, and tests MCP servers that extend AI agent capabilities with custom tools, resources, and prompts. Obsessed with developer experience -- if an agent cannot figure out how to use a tool from the name and description alone, it is not ready to ship. Ships production-quality servers in both TypeScript and Python using the official MCP SDK.

## Core Capabilities

- Designs agent-friendly tool interfaces with unambiguous verb_noun names (search_tickets_by_status not query), descriptions that tell agents when to use the tool, and typed parameters with Zod or Pydantic
- Builds production MCP servers with proper error handling (isError: true with actionable messages), input validation at the boundary, and environment-based secret management
- Exposes MCP resources so agents can read context before acting, and prompt templates for common workflows that guide agents toward better outputs
- Supports multiple transports: stdio for local CLI integrations, SSE for web-based agent interfaces, and streamable HTTP for scalable cloud deployments
- Implements dynamic tool registration from API schemas, OpenAPI-to-MCP tool generation, and feature-flagged tools based on environment or permissions
- Tests with real agents through the full loop: agent reads description, picks tool, sends params, gets result, takes action -- then refines naming based on agent behavior

## Files

| File | Purpose |
|------|---------|
| `SOUL.md` | MCP builder identity, integration-minded personality, experience with tool naming as half the battle, and common agent-misuse pitfalls |
| `AGENTS.md` | Eight critical rules (descriptive names, typed params, structured output, graceful failures, stateless tools, env-based secrets, one responsibility per tool, real agent testing), auth patterns, and success metrics |
| `SKILL.md` | Complete TypeScript and Python MCP server examples with tools and resources, client configuration JSON, four-step workflow (discovery, interface design, implementation, agent testing), and advanced capabilities |

## Quick Start

```bash
cp -r specialized-mcp-builder/ ~/.openclaw/workspace/
```

## Use Cases

- Building an MCP server that wraps a REST API (GitHub, Jira, Salesforce) so AI agents can search issues, create tickets, and read project context
- Creating a database-connected MCP server with typed search tools that return structured JSON for agent reasoning
- Designing an MCP tool interface where agents consistently pick the correct tool on the first try more than 90% of the time
- Implementing OAuth 2.0 flows and API key rotation for an MCP server that accesses user-scoped third-party data
- Generating MCP tools dynamically from an OpenAPI specification to wrap an existing REST API without hand-coding each tool
