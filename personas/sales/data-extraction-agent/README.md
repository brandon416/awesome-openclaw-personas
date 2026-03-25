# Sales Data Extraction Agent

An intelligent data pipeline specialist that monitors, parses, and extracts sales metrics from Excel files in real time. Watches designated directories for new or updated sales reports, extracts key metrics (Month to Date, Year to Date, Year End projections), normalizes data with flexible column mapping, and persists validated metrics to PostgreSQL with complete audit trails.

## Core Capabilities

- Monitors directories for new `.xlsx` and `.xls` files using filesystem watchers, ignoring temporary Excel lock files
- Maps columns flexibly using fuzzy matching (revenue/sales/total_sales, units/qty/quantity) to handle varying Excel formats
- Extracts MTD, YTD, and Year End metrics by detecting metric type from sheet names with sensible defaults
- Matches representatives by email or full name, logging warnings for unmatched rows without corrupting data
- Persists extracted metrics to PostgreSQL with transactions for atomicity and source file references for audit trails
- Calculates quota attainment automatically when both quota and revenue fields are present

## Files

| File | Purpose |
|------|--------|
| `SOUL.md` | Identity as precision-driven data pipeline specialist, core traits, adaptive column mapping philosophy |
| `AGENTS.md` | Critical rules (never overwrite, always log, flexible schemas), 8-step workflow process, success metrics |
| `SKILL.md` | Core mission (file monitoring, metric extraction, data persistence), technical specifications for file handling and database operations |

## Quick Start

```bash
cp -r sales-data-extraction-agent/ ~/.openclaw/workspace/
```

## Use Cases

- Automating extraction of monthly sales reports from Excel files into a live reporting dashboard
- Processing varying Excel formats from different regional sales teams with inconsistent column naming
- Building an audit trail for all sales data imports with file names, row counts, timestamps, and failure logs
- Feeding real-time MTD and YTD sales metrics to downstream reporting agents as soon as new files appear
- Calculating quota attainment across sales representatives from uploaded Excel reports without manual intervention
