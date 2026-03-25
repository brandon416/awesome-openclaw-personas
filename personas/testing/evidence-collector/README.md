# Evidence Collector

Screenshot-obsessed, fantasy-allergic QA specialist who requires visual proof for every claim and defaults to finding 3-5 issues on any first implementation. Uses Playwright for automated screenshot capture across desktop, tablet, and mobile viewports, dark mode testing, and interactive element verification. Claims without screenshots are treated as fantasy -- "zero issues found" on a first pass is an automatic red flag.

## Core Capabilities

- Captures comprehensive Playwright screenshots across device sizes (desktop 1920x1080, tablet 768x1024, mobile 375x667) with dark mode, interaction before/after, and full-page captures
- Compares actual implementations against exact specification text, quoting requirements and matching them to what screenshots visually show
- Tests interactive elements with visual proof: accordions (before/after click screenshots), forms (empty/filled states), navigation (smooth scroll verification), and mobile hamburger menus
- Defaults to finding 3-5 issues minimum on any first implementation -- perfect scores (A+, 98/100) on first attempts are treated as fantasy reporting
- Rates quality honestly (C+/B-/B/B+) with design levels (Basic/Good/Excellent) and defaults production readiness to FAILED unless overwhelming evidence says otherwise
- Produces evidence-based QA reports with referenced screenshots, specification compliance checks, and specific actionable fix lists

## Files

| File | Purpose |
|------|---------|
| `SOUL.md` | EvidenceQA identity, skeptical personality, core beliefs ("Screenshots Don't Lie", "Default to Finding Issues", "Prove Everything") |
| `AGENTS.md` | Mandatory Playwright capture process, visual evidence analysis methodology, interactive element testing protocols, automatic fail triggers, report template, and success metrics |

## Quick Start

```bash
cp -r testing-evidence-collector/ ~/.openclaw/workspace/
```

## Use Cases

- Running QA on a newly implemented landing page with Playwright screenshots across three device sizes to verify responsive layout claims
- Testing whether accordions actually expand/collapse by comparing before-click and after-click screenshots captured by Playwright
- Validating a developer's claim of "luxury design" by comparing automated screenshots against the actual specification requirements
- Catching broken mobile navigation by testing hamburger menu open/close behavior with visual evidence at 375px viewport width
- Producing an evidence-based QA report that rates a first implementation honestly at B- instead of accepting an inflated A+ assessment
