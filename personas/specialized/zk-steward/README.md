# ZK Steward

Knowledge-base steward in the spirit of Niklas Luhmann's Zettelkasten that turns complex tasks into organic parts of a knowledge network. Default perspective is Luhmann; switches to domain experts (Feynman for learning, Munger for strategy, Ogilvy for brand, Karpathy for engineering) by task. Enforces atomic notes, connectivity with at least 2 meaningful links, and validation loops at every closure.

## Core Capabilities

- Validates every note against Luhmann's four principles: Atomicity (understood alone?), Connectivity (2+ meaningful links?), Organic growth (over-structure avoided?), and Continued dialogue (sparks further thinking?)
- Switches domain perspectives using a triangulation of domain, task type, and output form -- mapping to experts like Munger (mental models, inversion), Feynman (first principles), Sugarman (copy triggers), or Mollick (AI prompts)
- Runs a link-proposer flow for new notes: suggests link candidates, keyword/index entries, and one Gegenrede (counter-question from a different discipline) to spark cross-domain dialogue
- Maintains daily logs (Intent / Changes / Open loops), promotes easy-to-forget items to an open-loops file, and syncs evergreen knowledge to persistent memory
- Produces structure notes for deep reading (books, long articles) with overview questions, logic trees linking to atomic notes, and reading sequences
- Follows a filing decision tree using time-based paths (YYYY/MM/YYYYMMDD/) and ensures index entries are entry points, not categories -- one note can sit under multiple indices

## Files

| File | Purpose |
|------|---------|
| `SOUL.md` | ZK Steward identity, Luhmann-inspired personality, domain thinking with expert-level conditioning, and indexing philosophy |
| `AGENTS.md` | Non-negotiable rules (every reply addresses user by name, states expert perspective), Luhmann's four-principle validation gate, execution discipline, workflow steps, and success metrics |
| `SKILL.md` | Knowledge network building methodology, domain-expert mapping table (9 domains), task closure checklist, file naming convention, daily log template, structure note example, and companion skill descriptions |

## Quick Start

```bash
cp -r zk-steward/ ~/.openclaw/workspace/
```

## Use Cases

- Building a personal knowledge base with atomic notes and explicit linking following Zettelkasten principles, with validation at every note closure
- Processing a book or long technical article into a structure note with atomic sub-notes, logic trees, and reading sequences using the deep-learning flow
- Analyzing a business strategy question from Charlie Munger's mental models perspective, then adding a Gegenrede counter-question from a competing discipline
- Maintaining a daily knowledge log that tracks intent, changes, and open loops, with automatic promotion of easy-to-forget items
- Creating cross-domain connections between engineering notes and marketing insights through the link-proposer flow with keyword and index suggestions
