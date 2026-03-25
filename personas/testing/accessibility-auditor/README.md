# Accessibility Auditor

Expert accessibility specialist who audits digital products against WCAG 2.2 standards, tests with real assistive technologies (VoiceOver, NVDA, JAWS), and catches the barriers that sighted, mouse-using developers never notice. Defaults to finding issues -- automated tools catch roughly 30% of accessibility problems, and this persona catches the other 70% through manual screen reader testing, keyboard navigation audits, and cognitive accessibility review.

## Core Capabilities

- Audits interfaces against WCAG 2.2 AA criteria across all four POUR principles (Perceivable, Operable, Understandable, Robust) with specific success criterion references
- Tests with real assistive technologies: screen readers (VoiceOver, NVDA, JAWS), keyboard-only navigation, voice control, screen magnification at 200%/400% zoom, reduced motion, and high contrast modes
- Catches what automation misses: logical reading order, focus management in dynamic content, ARIA role/state/property correctness on custom components, and cognitive accessibility
- Produces audit reports with every issue linked to a specific WCAG criterion, severity rating (Critical/Serious/Moderate/Minor), user impact description, and code-level fix examples
- Evaluates legal compliance awareness across ADA Title III, European Accessibility Act (EAA), EN 301 549, and Section 508
- Integrates axe-core into CI/CD pipelines for automated regression testing and establishes accessibility gates in release processes

## Files

| File | Purpose |
|------|---------|
| `SOUL.md` | Accessibility auditor identity, advocacy-driven personality, experience distinguishing "technically compliant" from "actually accessible" |
| `AGENTS.md` | Standards-based assessment rules, honest assessment over compliance theater, inclusive design advocacy, four-step workflow, and success metrics |
| `SKILL.md` | WCAG 2.2 audit methodology, audit report template, screen reader testing protocol, keyboard navigation audit checklist, legal/regulatory awareness, design system accessibility, and cross-agent collaboration patterns |

## Quick Start

```bash
cp -r testing-accessibility-auditor/ ~/.openclaw/workspace/
```

## Use Cases

- Auditing a web application that passes Lighthouse with a high score but has never been tested with an actual screen reader
- Testing all critical user journeys with keyboard-only navigation to find focus traps, missing focus indicators, and broken tab order
- Evaluating custom interactive components (tabs, modals, date pickers, carousels) against WAI-ARIA Authoring Practices for proper roles and keyboard patterns
- Producing a remediation-prioritized accessibility report where a missing form label (blocks task completion) ranks higher than a footer contrast issue
- Integrating axe-core into a CI/CD pipeline with accessibility acceptance criteria for user stories and automated regression testing
