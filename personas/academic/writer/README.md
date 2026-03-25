# Writer

The paper writing core of the OpenClaw multi-agent academic system. Produces top-conference-quality academic papers with native-level English, precise LaTeX typesetting (ACL, NeurIPS, ICML, ICLR templates), and compelling narrative structure that transforms technical contributions into Oral-worthy stories.

## Core Capabilities

- Writes native-level academic English with systematic weak-to-strong expression upgrades (e.g., "is better than" to "consistently outperforms") and logical topic-sentence paragraph construction
- Masters standard paper structure: five-part abstract, hook-to-contribution introduction, thematic Related Work, intuition-first Method, analysis-rich Experiments, and honest Conclusion
- Produces publication-ready LaTeX with booktabs tables, properly placed captions, cross-references, and venue-specific formatting (ACL 8-page limit, NeurIPS style)
- Frames contributions to avoid both overclaim and underclaim, with precise novelty statements that clearly explain "what is new and why"
- Integrates outputs from all other agents: experiment tables from Coder, Related Work drafts from Surveyor, motivation narratives from Ideator
- Runs self-check writing quality checklists covering story line coherence, contribution support, quantitative results in abstract, and format compliance

## Files

| File | Purpose |
|------|--------|
| `SOUL.md` | Writing expert identity, section-by-section guides, expression optimization dictionary, quality checklist |
| `AGENTS.md` | Model config, draft version tracking, style guide maintenance, Reviewer/Critic feedback integration |
| `USER.md` | Research domain (AI/NLP/Multi-Agent), clear concise style preference, ACL/NeurIPS LaTeX templates |

## Quick Start

```bash
cp -r academic-writer/ ~/.openclaw/workspace/
```

## Use Cases

- Draft a complete ACL paper from outline to camera-ready, section by section, following the five-part abstract and hook-driven introduction structure
- Rewrite a weak Introduction to create a compelling motivation narrative that grabs the reviewer within the first three sentences
- Convert raw experiment results from the Coder agent into a properly formatted Experiments section with analysis, not just numbers
- Polish a paper draft by upgrading weak academic expressions and ensuring paragraph transitions create a coherent narrative flow
- Prepare the final camera-ready version with correct LaTeX formatting, booktabs tables, and BibTeX references for the target venue
