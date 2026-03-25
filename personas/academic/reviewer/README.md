# Reviewer

The quality gatekeeper of the OpenClaw multi-agent academic system. Simulates a senior reviewer at ACL, NeurIPS, or ICML Area Chair level, scoring papers across six dimensions (soundness, novelty, significance, clarity, reproducibility, experiments), identifying dealbreaker weaknesses, and providing actionable rebuttal strategies. Holds veto power over paper submission.

## Core Capabilities

- Performs comprehensive reviews scoring soundness, novelty, significance, clarity, reproducibility, and experimental rigor on a 1-10 scale with severity-tagged weaknesses (fatal/important/minor)
- Detects dealbreaker weaknesses: missing key baselines, insufficient novelty, dataset-claim mismatches, formula errors, and overlooked related work
- Prepares rebuttal strategies that distinguish between legitimate criticism, misunderstandings, and out-of-scope requests, with prioritized response plans
- Benchmarks papers against recent accept/reject decisions at the target venue to calibrate expectations
- Runs camera-ready checks including format compliance, anonymity verification, figure/table reference correctness, and PDF metadata cleaning
- Applies venue-specific review standards (ACL focus on error analysis and broader impact; NeurIPS focus on theoretical depth and scalability)

## Files

| File | Purpose |
|------|--------|
| `SOUL.md` | Reviewer identity, comprehensive review methodology, rebuttal preparation, venue-specific standards |
| `AGENTS.md` | Model config, veto power authority, review iteration tracking, quality gate enforcement |
| `USER.md` | Research domain (AI/NLP/Multi-Agent), constructive-but-rigorous review style, venue calibration |

## Quick Start

```bash
cp -r academic-reviewer/ ~/.openclaw/workspace/
```

## Use Cases

- Get a full internal review of your paper draft before submission to identify fatal weaknesses while there is still time to fix them
- Prepare a rebuttal strategy after receiving real reviewer comments, distinguishing valid criticism from misunderstandings
- Check whether your experimental baselines are sufficient for the target venue or if critical comparisons are missing
- Run a camera-ready compliance check to catch anonymity leaks, format violations, and broken references before the final upload
- Calibrate your paper's contribution level against recent accept decisions at ACL or NeurIPS to set realistic expectations
