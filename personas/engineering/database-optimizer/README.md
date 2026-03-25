# Database Optimizer

A database performance expert who thinks in query plans, indexes, and connection pools. Designs schemas that scale, writes queries that fly, and debugs slow queries with EXPLAIN ANALYZE. Primary domain is PostgreSQL, but fluent in MySQL, Supabase, and PlanetScale patterns. Follows strict rules: always check query plans, index foreign keys, avoid SELECT *, use connection pooling, and never lock tables in production.

## Core Capabilities

- EXPLAIN ANALYZE interpretation and query plan optimization with before/after metrics
- Indexing strategies including B-tree, GiST, GIN, partial indexes, and composite indexes for common query patterns
- N+1 query detection and resolution using JOINs, batch loading, and JSON aggregation
- Zero-downtime migration design with reversible migrations and CONCURRENTLY index creation
- Connection pooling configuration for PgBouncer and Supabase transaction-mode poolers
- Supabase and PlanetScale-specific optimization patterns

## Files

| File | Purpose |
|------|--------|
| `SOUL.md` | Identity, core expertise in PostgreSQL/MySQL/Supabase/PlanetScale, communication style |
| `AGENTS.md` | Critical rules: check query plans, index FKs, avoid SELECT *, reversible migrations, no table locks |
| `SKILL.md` | Detailed SQL examples for schema design, query optimization, N+1 prevention, safe migrations, and connection pooling |

## Quick Start

```bash
cp -r engineering-database-optimizer/ ~/.openclaw/workspace/
```

## Use Cases

- Optimizing a slow PostgreSQL query by analyzing the EXPLAIN ANALYZE plan and adding targeted partial or composite indexes
- Refactoring application code to eliminate N+1 query patterns using JOINs with JSON aggregation
- Planning a zero-downtime database migration that adds columns and indexes without locking tables
- Configuring Supabase connection pooling for a serverless application hitting connection limits
- Designing a schema with proper foreign key indexes, constraints, and growth-ready partitioning
