# Executive Summary Generator

Consultant-grade AI specialist that thinks and communicates like a senior strategy consultant with Fortune 500 experience. Transforms complex business inputs into concise, actionable executive summaries (325-475 words) using McKinsey SCQA, BCG Pyramid Principle, and Bain action-oriented recommendation frameworks, enabling C-suite decision-makers to grasp essence, evaluate impact, and decide next steps in under three minutes.

## Core Capabilities

- Structures every summary using McKinsey's SCQA (Situation-Complication-Question-Answer) framework with BCG Pyramid Principle for top-down logical flow
- Enforces strict output format: Situation Overview (50-75 words), Key Findings (125-175 words with quantified data points), Business Impact (50-75 words), Recommendations (75-100 words), and Next Steps (25-50 words)
- Requires every key finding to include at least one quantified or comparative data point with bold strategic implications ordered by business impact
- Tags recommendations with priority levels (Critical/High/Medium) and attaches specific owner, timeline, and expected result to each
- Maintains analytical rigor through scenario analysis (best/worst/likely), ROI/NPV calculations, and value-vs-effort prioritization matrices
- Refuses to make assumptions beyond provided data, explicitly flagging data gaps and uncertainties

## Files

| File | Purpose |
|------|--------|
| `SOUL.md` | Consultant identity, analytical/decisive personality, SCQA framework reference, quality standards |
| `AGENTS.md` | Communication rules, workflow process (intake, structure, generate, QA), executive summary template, consulting framework mastery |
| `SKILL.md` | Core mission (think like a consultant, transform complexity), required output format with word counts, advanced analytical capabilities |

## Quick Start

```bash
cp -r support-executive-summary-generator/ ~/.openclaw/workspace/
```

## Use Cases

- Condense a 40-page quarterly business review into a 400-word executive summary that the CEO can act on in three minutes
- Transform raw customer analytics data into a strategic brief with quantified findings and prioritized recommendations for the CMO
- Prepare a board-ready summary of a proposed acquisition with financial impact, risk magnitude, and decision deadlines
- Convert a lengthy market research report into an actionable SCQA-structured brief with specific owner assignments and 30-day next steps
- Generate a crisis response summary that quantifies the business exposure and presents prioritized mitigation actions with clear accountability
