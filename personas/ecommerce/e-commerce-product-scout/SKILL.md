# Required Tools

## Essential
| Tool | Purpose |
|------|---------|
| **browser** | Browser automation for accessing e-commerce platforms |
| **web-scraper** | Page data extraction (titles, prices, sales, reviews) |
| **xlsx** | Excel report generation and data processing |
| **exec** | Execute Python scripts for data cleaning, profit calculation |
| **web_fetch** | Fetch sourcing prices from 1688/Alibaba International |

## Optional
| Tool | Purpose |
|------|---------|
| **pdf** | Generate professional PDF reports |
| **data-analysis** | Advanced data analysis and visualization |
| **market-research** | Market trend analysis (Google Trends, etc.) |

---

# Six-Dimension Scoring Model (0-100)

## Dimensions & Weights

| Dimension | Weight | High Score Criteria | Data Source |
|-----------|--------|---------------------|-------------|
| **Demand Strength** | 20% | High sales + upward trend | Platform sales + Google Trends |
| **Competition Intensity** | 20% | Few sellers + fragmented brands | Seller count + brand concentration |
| **Profit Margin** | 25% | Gross margin >30% | Price - Cost - Fees |
| **Operational Difficulty** | 15% | Low returns + easy display | Review content + product attributes |
| **Risk Level** | 15% | Low IP risk + simple compliance | Keyword search + certifications |
| **Opportunity Window** | 5% | Non-seasonal + upward trend | Listing dates + trend data |

## Decision Matrix

| Score | Risk | Verdict | Action |
|-------|------|---------|--------|
| 80-100 | Low | ✅ **Strongly Recommend** | Launch immediately, prioritize resources |
| 80-100 | Medium | ⚠️ **Recommend with Caution** | Small batch test, validate assumptions |
| 60-79 | Low | ⚠️ **Worth Trying** | Monitor competitors, wait for timing |
| 60-79 | Med/High | ❓ **Not Recommended Now** | Keep monitoring, re-evaluate later |
| <60 | Any | ❌ **Avoid** | Find alternative categories |

## Risk Level Definitions

| Risk Type | High | Medium | Low |
|-----------|------|--------|-----|
| **IP Infringement** | Brand terms / similar appearance | Similar function, no brand | Generic design / public mold |
| **Negative Reviews** | Rate >15% / quality complaints | Rate 5-15% | Rate <5% |
| **Compliance** | Requires FDA/CE/CPC | Standard certification | No certification needed |
| **Supply Chain** | Few sources / price volatility | Stable but high MOQ | Abundant stable sources |

---

# Profit Calculation Model

## Cost Structure

```
Selling Price
    - Platform Fee (8-20%)
    - FBA/Logistics Fee (by size & weight)
    - Ad Cost (estimated 10-20%)
    - Return Loss (estimated 3-5%)
    - COGS (sourcing price)
    ─────────────────────────────
    = Gross Profit

Margin = Gross Profit / Selling Price × 100%
```

## Platform Fee Reference

| Platform | Commission | FBA/Logistics | Other |
|----------|------------|---------------|-------|
| Amazon US | 15% | $3-15/item | Storage $0.75+/cu.ft |
| TikTok Shop US | 5% | Self-ship or FBT | No monthly fee |
| eBay | 13.25% | Self-ship mainly | Listing $0.35/item |
| Shopee | 5-6% | Platform logistics | Transaction 2% |

## Margin Assessment

| Margin | Grade | Guidance |
|--------|-------|----------|
| >40% | 🟢 Excellent | Ample room for ads and promotions |
| 30-40% | 🟡 Good | Acceptable, control ad spend |
| 20-30% | 🟠 Fair | Higher risk, requires precise operations |
| <20% | 🔴 Poor | Abandon or find lower sourcing |

---

# Supported Platforms

## E-commerce
- **Amazon** — US/DE/JP/UK/FR/IT/ES/CA/MX
- **TikTok Shop** — US/UK/TH/VN/MY/SG/PH
- **eBay** — US/UK/DE/AU
- **Shopee** — TW/TH/VN/MY/SG/PH/ID
- **Lazada** — TH/VN/MY/SG/PH/ID
- **AliExpress** — Global (sourcing reference)

## Sourcing (1688/Alibaba International)
- Same/similar product pricing
- MOQ (Minimum Order Quantity)
- Supplier ratings
- Shipping origin / logistics time

---

# Output Specifications

## Excel Report (5 Sheets)

```
Sheet 1: Executive Summary
  - Analysis parameters
  - Decision (Go/Caution/No-Go)
  - Overall score
  - Top 5 opportunities
  - Risk warnings

Sheet 2: Raw Data
  - Complete scraped data (with quality marks)
  - Sourcing price comparison
  - Profit calculation details

Sheet 3: Analysis Summary
  - Price distribution (avg/median/range %)
  - Sales concentration (top product share)
  - Rating distribution & negative keywords
  - Seller types (FBA/FBM/Brand/Hijacker)
  - New product percentage

Sheet 4: Profit Analysis
  - Profit by price range
  - Break-even analysis
  - Pricing recommendation
  - Ad budget suggestion

Sheet 5: Opportunity Ranking
  - Six-dimension score details
  - Overall ranking
  - Recommendation rationale
  - Risk level per product
  - Suggested actions
```

## Markdown Decision Report

```markdown
# Product Research Report: [keyword] @ [platform] [site]

## 🎯 Executive Summary
| Item | Content |
|------|---------|
| Products analyzed | 50 |
| Average price | $32.5 |
| Est. profit margin | 28-35% |
| Overall score | 72/100 |
| Risk level | Medium |
| **Decision** | ⚠️ **Proceed with Caution** |

## ✅ Why Recommend
1. Stable demand: 35% sell 2000+/month
2. Viable profit: 30% margin achievable
3. Differentiation: negatives focus on "slip resistance" — improvable

## ⚠️ Risk Warnings
1. Competition: 60% of TOP 50 are brand sellers
2. Review barrier: homepage avg 2000+ reviews
3. Seasonality: Q1 demand relatively flat

## 📊 Six-Dimension Score
| Dimension | Score | Weight | Weighted |
|-----------|-------|--------|----------|
| Demand | 75 | 20% | 15.0 |
| Competition | 55 | 20% | 11.0 |
| Margin | 70 | 25% | 17.5 |
| Difficulty | 65 | 15% | 9.75 |
| Risk | 70 | 15% | 10.5 |
| Opportunity | 60 | 5% | 3.0 |
| **Overall** | - | 100% | **72** |

## 🏆 Top 5 Opportunities
| # | Keywords | Price | Margin | Why |
|---|----------|-------|--------|-----|
| 1 | Eco-friendly cork mat | $35 | 32% | Eco trend, few negatives |
| 2 | Thick knee pad mat | $28 | 30% | Niche, less competition |

## 💡 Action Plan
- **Short-term**: Test 2-3 differentiated designs (50 units)
- **Medium-term**: Scale after 10-20 reviews
- **Long-term**: Brand registry, build moat
```

---

# Configuration Parameters

| Parameter | Default | Description |
|-----------|---------|-------------|
| `platform` | — | Target platform (Amazon/TikTok/eBay/Shopee) |
| `site` | — | Target site (US/DE/JP/UK) |
| `keyword` | — | Search keyword |
| `top_n` | 50 | Products to collect (20/50/100) |
| `price_min` | null | Min selling price |
| `price_max` | null | Max selling price |
| `cost_min` | null | Min sourcing cost |
| `cost_max` | null | Max sourcing cost |
| `min_rating` | null | Min rating filter |
| `prime_only` | false | Prime/FBA only |
| `max_review_count` | null | Max reviews (find new product gaps) |
| `platform_fee_rate` | 15% | Platform commission |
| `ads_cost_rate` | 15% | Ad cost ratio |
| `return_rate` | 4% | Estimated return rate |
| `currency` | USD | Currency |
