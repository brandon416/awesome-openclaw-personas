# Scout

The academic intelligence officer of the OpenClaw multi-agent system. Continuously monitors arXiv, Semantic Scholar, top conference proceedings, and lab blogs to deliver daily paper digests with relevance scoring, weekly trend analysis, competitive intelligence on rival research groups, and urgent collision alerts when published work overlaps with ongoing research.

## Core Capabilities

- Delivers daily paper digests (3-5 papers) with one-sentence summaries, relevance scores (1-5), and reading priority from arXiv (cs.CL, cs.AI, cs.LG, cs.MA), Semantic Scholar, and top conference accepted lists
- Performs weekly and monthly trend analysis identifying rising/declining research directions, emerging keywords, and paradigm shifts
- Tracks competitive intelligence on key research groups (DeepMind, OpenAI, Anthropic, Meta FAIR, Tsinghua, CMU, Stanford, Berkeley) and flags potential collision risks
- Issues urgent alerts when a new publication closely overlaps with the team's in-progress research, triggering immediate strategy review
- Monitors conference deadlines, notification dates, and workshop CFPs with countdown tracking
- Tracks open-source project updates and framework releases relevant to the research stack (PyTorch, Transformers, vLLM)

## Files

| File | Purpose |
|------|--------|
| `SOUL.md` | Intelligence officer identity, daily/weekly report templates, keyword monitoring config, alert escalation protocol |
| `AGENTS.md` | Model config, browser tool access, digest queue management, inter-agent alert routing |
| `USER.md` | Research domain (AI/NLP/Multi-Agent), concise digest format preference, arXiv/Semantic Scholar sources |

## Quick Start

```bash
cp -r academic-scout/ ~/.openclaw/workspace/
```

## Use Cases

- Get a daily curated feed of the most relevant new papers in multi-agent reasoning without manually browsing arXiv
- Receive an immediate alert if a competing group publishes work that overlaps with your current research direction
- Review a weekly trend report to decide whether your research direction is gaining or losing community momentum
- Track upcoming conference deadlines and plan submission timelines months in advance
- Monitor when key rival labs release new preprints or open-source tools that could affect your experimental baselines
