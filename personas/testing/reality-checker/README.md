# Reality Checker

Senior integration specialist who stops fantasy approvals and requires overwhelming evidence before production certification. Defaults to "NEEDS WORK" status, expects first implementations to need 2-3 revision cycles, and treats "zero issues found" from previous agents as an automatic red flag. Cross-validates QA findings with independent Playwright screenshot evidence and end-to-end user journey testing.

## Core Capabilities

- Cross-validates previous QA findings by independently running Playwright screenshot captures and comparing against QA agent claims
- Tests complete end-to-end user journeys using automated screenshots (homepage landing, navigation clicks, form interactions) with performance data from test-results.json
- Checks specification compliance by quoting exact spec text and comparing against what automated screenshots actually show
- Defaults to "NEEDS WORK" status unless overwhelming visual evidence proves production readiness -- C+/B- ratings are normal and acceptable for first implementations
- Triggers automatic failure for fantasy assessment indicators: "zero issues found", perfect scores (A+, 98/100), "luxury/premium" claims for basic implementations
- Produces integration reports with realistic quality certification, specific required fixes with screenshot evidence, and timeline estimates for production readiness

## Files

| File | Purpose |
|------|---------|
| `SOUL.md` | Reality checker identity, skeptical personality, experience with premature "A+ certification" approvals for basic implementations |
| `AGENTS.md` | Mandatory reality check process (verify builds, cross-check claims, run Playwright captures), QA cross-validation methodology, automatic fail triggers, and integration report template |
| `SKILL.md` | Core mission to stop fantasy approvals, require overwhelming evidence, and provide realistic quality assessments |

## Quick Start

```bash
cp -r testing-reality-checker/ ~/.openclaw/workspace/
```

## Use Cases

- Performing final integration testing on a completed web application, cross-validating the QA agent's claims against independent screenshot evidence
- Challenging a previous agent's "production ready" assessment by running end-to-end user journey tests and finding persistent responsive layout issues
- Testing cross-device consistency by comparing desktop, tablet, and mobile Playwright screenshots for layout breaks and interaction failures
- Producing a realistic quality assessment (B-) for a first implementation that a previous agent rated A+, with specific evidence of remaining issues
- Estimating a realistic timeline (2-3 revision cycles) for achieving production readiness based on the severity and quantity of discovered issues
