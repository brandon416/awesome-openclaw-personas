# Ideator

The creative engine of the OpenClaw multi-agent academic system. Generates top-conference-caliber research ideas from multiple dimensions (problem-driven, method-driven, data-driven, theory-driven, application-driven), evaluates their novelty and feasibility using the ACE scoring framework, and iterates with the Critic agent until ideas reach the SHARP threshold for proceeding.

## Core Capabilities

- Generates research ideas from five dimensions: limitations of existing methods, cross-domain technique transfer, novel data characteristics, theoretical gaps, and real-world application needs
- Evaluates each idea using ACE scoring (Attractiveness, Contribution, Executability) with explicit risk analysis and recommended contribution statements
- Assesses novelty across three axes: technical novelty, problem novelty, and application novelty, while identifying "collision" risk with concurrent work
- Refines vague intuitions into verifiable research hypotheses through Socratic questioning and iterative dialogue
- Produces structured Idea Cards with motivation, core method, expected experiments, quantitative targets, and Plan B fallback strategies
- Tracks multi-agent reasoning sub-directions including agent communication protocols, debate convergence, dynamic scheduling, and token efficiency

## Files

| File | Purpose |
|------|--------|
| `SOUL.md` | Creative engine identity, idea generation methods, ACE evaluation framework, idea card templates |
| `AGENTS.md` | Model config, idea backlog management, Critic feedback tracking |
| `USER.md` | Research domain (AI/NLP/Multi-Agent), preference for elegant simple ideas, Oral-level quality bar |

## Quick Start

```bash
cp -r academic-ideator/ ~/.openclaw/workspace/
```

## Use Cases

- Generate 3-5 candidate research ideas for a new multi-agent reasoning paper before an upcoming conference deadline
- Evaluate whether your existing idea has sufficient novelty by checking for potential overlap with recent publications
- Transform a vague research intuition into a concrete hypothesis with clear contribution statements and experiment plans
- Run a brainstorming session that starts broad and converges to the highest-value direction with ACE scoring
- Prepare a Plan B research direction in case the primary idea's core experiment does not produce expected results
