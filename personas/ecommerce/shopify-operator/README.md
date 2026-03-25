# Shopify Operator

A hands-on Shopify store coach that takes new sellers from zero to a live, decorated store with real products. Executes a complete 5-stage pipeline: theme-based product sourcing (Jungle Scout + Alibaba), bulk listing with SEO optimization, store decoration with hero banners and lifestyle images, social media marketing (X + Instagram), and daily monitoring with cron-driven competitor tracking and strategy digests.

## Core Capabilities

- **5-stage end-to-end SOP** — sourcing → listing → decoration → social marketing → daily monitoring, with strict phase gating between stages
- **Anti-hallucination rules** — source isolation between Jungle Scout and Alibaba data, URL attribution verification, image URL validation, no cross-source fabrication
- **Real supplier evidence** — every product recommendation traces back to actual Alibaba/1688 listings with unit cost, MOQ, and margin math
- **Shopify API execution** — creates products, uploads images, configures themes, sets announcement bars, and publishes directly via API
- **Social media marketing** — generates Twitter + Instagram content with authorization flow, image generation, and automated posting
- **Daily cron monitoring** — competitor tracking, traffic/sales digests, weekly product optimization, and strategy summaries

## Files

| File | Purpose |
|------|---------|
| `SOUL.md` | Hands-on coaching personality, data integrity principles, anti-hallucination rules |
| `AGENTS.md` | Complete 5-stage SOP with phase gating, API parameters, and social media workflow |
| `IDENTITY.md` | Role definition and beginner-friendly communication style |
| `BOOTSTRAP.md` | First-run onboarding flow |
| `USER.md` | User profile template |
| `TOOLS.md` | Tool configuration notes |

## Quick Start

```bash
cp -r shopify-operator/ ~/.openclaw/workspace/
```

## Use Cases

- Launch a new Shopify store from scratch with real sourced products and professional decoration
- Research profitable product niches using Jungle Scout data and find matching Alibaba suppliers with margin analysis
- Bulk-list products with SEO titles, lifestyle images, and proper pricing with compare-at discounts
- Set up automated daily competitor monitoring and weekly strategy digests via cron tasks
- Create and publish social media launch campaigns on X and Instagram with generated marketing visuals
