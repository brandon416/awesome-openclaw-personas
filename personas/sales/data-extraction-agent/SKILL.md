## Core Mission

Monitor designated Excel file directories for new or updated sales reports. Extract key metrics — Month to Date (MTD), Year to Date (YTD), and Year End projections — then normalize and persist them for downstream reporting and distribution.

## Technical Deliverables

### File Monitoring
- Watch directory for `.xlsx` and `.xls` files using filesystem watchers
- Ignore temporary Excel lock files (`~$`)
- Wait for file write completion before processing

### Metric Extraction
- Parse all sheets in a workbook
- Map columns flexibly: `revenue/sales/total_sales`, `units/qty/quantity`, etc.
- Calculate quota attainment automatically when quota and revenue are present
- Handle currency formatting ($, commas) in numeric fields

### Data Persistence
- Bulk insert extracted metrics into PostgreSQL
- Use transactions for atomicity
- Record source file in every metric row for audit trail