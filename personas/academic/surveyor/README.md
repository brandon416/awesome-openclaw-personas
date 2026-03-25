# Surveyor

The knowledge engine of the OpenClaw multi-agent academic system. Conducts systematic literature reviews, produces standardized paper analysis cards, identifies research gaps through cross-paper comparison, and drafts Related Work sections with proper BibTeX citations in ACL Anthology format.

## Core Capabilities

- Performs systematic literature searches expanding keywords to synonyms, sub/super-concepts, and related terms, then snowballing through citation graphs to catch missed work
- Produces standardized paper analysis cards covering motivation, problem formulation, method, experiments, ablation findings, limitations, and impact assessment
- Identifies research gaps by cross-comparing multiple papers to find unsolved problems and distinguish incremental improvements from breakthrough opportunities
- Drafts Related Work sections organized by thematic groups with clear differentiation from the user's contribution
- Maintains reading priority lists (must-read foundational, important recent SOTA, reference) with BibTeX entries in ACL Anthology format
- Tracks multi-agent sub-directions including debate convergence, communication protocols, agent orchestration frameworks, and token-efficient reasoning

## Files

| File | Purpose |
|------|--------|
| `SOUL.md` | Literature expert identity, paper analysis framework, gap identification methodology, citation standards |
| `AGENTS.md` | Model config, browser tool for paper retrieval, curated paper database with tags and relevance scores |
| `USER.md` | Research domain (AI/NLP/Multi-Agent), comprehensive 2-3 year coverage depth, Semantic Scholar/arXiv/ACL Anthology sources |

## Quick Start

```bash
cp -r academic-surveyor/ ~/.openclaw/workspace/
```

## Use Cases

- Conduct a full literature survey on multi-agent debate methods before starting a new research project
- Verify whether a proposed research idea has already been published by checking seminal and recent papers in the area
- Generate a draft Related Work section with thematic groupings and proper BibTeX citations for your paper
- Identify the current SOTA methods and benchmarks in a specific sub-field to design fair experimental comparisons
- Map the development timeline of a research direction to understand where the field is heading and where opportunities remain
