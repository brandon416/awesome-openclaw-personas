# Document Generator

Specialist in creating professional documents programmatically using code-based approaches. Generates PDFs, presentations (PPTX), spreadsheets (XLSX), and Word documents (DOCX) with proper formatting, charts, data visualization, and consistent branding -- accepting data as input and producing publication-ready documents as output through reusable template functions.

## Core Capabilities

- Generates PDFs using reportlab, weasyprint, fpdf2 (Python) or puppeteer HTML-to-PDF, pdf-lib, pdfkit (Node.js) for complex layouts and data reports
- Creates data-driven PPTX presentations with python-pptx or pptxgenjs using template-based slides with consistent branding
- Builds formatted XLSX spreadsheets with openpyxl, xlsxwriter, or exceljs including formulas, charts, and pivot-ready layouts
- Produces DOCX documents with python-docx or the docx Node.js package using styles, headers, table of contents, and consistent formatting
- Enforces accessibility standards with alt text, proper heading hierarchy, and tagged PDFs
- Builds reusable template functions rather than one-off scripts, with data-driven generation patterns

## Files

| File | Purpose |
|------|---------|
| `SOUL.md` | Document generator identity, format-savvy personality, experience with investor decks to compliance reports |
| `AGENTS.md` | Rules for proper styles (no hardcoded fonts), consistent branding, accessibility, reusable templates, and communication style |
| `SKILL.md` | Core mission with specific libraries per format (PDF, PPTX, XLSX, DOCX) for both Python and Node.js ecosystems |

## Quick Start

```bash
cp -r specialized-document-generator/ ~/.openclaw/workspace/
```

## Use Cases

- Generating a quarterly investor deck from a data source with consistent branding, charts, and formatted slides using python-pptx
- Creating automated compliance reports as tagged, accessible PDFs from database query results using weasyprint or puppeteer
- Building a reusable spreadsheet template with formulas, conditional formatting, and charts for monthly financial reporting
- Producing a batch of formatted Word documents (contracts, proposals) from a data template with proper styles and table of contents
- Converting HTML+CSS layouts into publication-ready PDFs for complex multi-column report designs
