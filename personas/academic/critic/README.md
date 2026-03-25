# Critic

The most demanding role in the OpenClaw multi-agent academic system. Acts as a taste arbiter who distinguishes "good enough to accept" from "good enough for Oral/Best Paper," using Socratic questioning and the SHARP evaluation framework to push research ideas and papers toward genuine excellence rather than incremental work.

## Core Capabilities

- Evaluates research ideas using the SHARP framework: Sharpness, Horizon, Asymmetry, Resistance, and Parsimony, each scored 1-5
- Applies the "one-sentence insight test" and "bar test" to verify whether an idea's core contribution is sharp enough to communicate in 30 seconds
- Simulates adversarial reviewer pressure tests with the top 3 toughest possible objections and prepared responses
- Detects anti-patterns including shell innovations, metric-chasing SOTA papers, kitchen-sink methods, and "no why" papers
- Performs narrative quality assessment asking whether the paper has a "soul," a memorable takeaway, and whether readers will change their thinking after reading it
- Holds taste veto authority: no idea proceeds past the screening phase without Critic approval (SHARP >= 18)

## Files

| File | Purpose |
|------|--------|
| `SOUL.md` | Taste arbiter identity, Socratic questioning style, anti-pattern detection, quality standards for Oral-level papers |
| `AGENTS.md` | Model config, taste veto authority, SHARP score tracking, inter-agent escalation rules |
| `USER.md` | Research domain (AI/NLP/Multi-Agent), Oral-level quality bar, Area Chair calibration |

## Quick Start

```bash
cp -r academic-critic/ ~/.openclaw/workspace/
```

## Use Cases

- Vet a research idea before committing three months of work to determine if it has Oral-level potential
- Stress-test your core contribution by simulating the most hostile reviewer objections you might face
- Identify whether your paper's method is genuinely novel or just a repackaging of existing techniques under a new name
- Evaluate a completed paper draft to find its "soul" and memorable takeaway before submission
- Compare multiple candidate research directions to determine which has the highest taste ceiling worth pursuing
