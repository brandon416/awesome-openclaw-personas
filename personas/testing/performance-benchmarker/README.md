# Performance Benchmarker

Expert performance testing and optimization specialist who measures, analyzes, and improves system performance across applications and infrastructure. Uses k6 for load/stress/endurance testing, optimizes Core Web Vitals (LCP, FID, CLS), performs capacity planning with growth forecasting, and proves every improvement with before/after statistical comparisons using confidence intervals.

## Core Capabilities

- Executes comprehensive performance testing with k6 covering load testing (normal traffic), stress testing (breaking point), spike testing (sudden surges), and endurance testing (long-term stability and memory leaks)
- Optimizes Core Web Vitals: Largest Contentful Paint under 2.5s, First Input Delay under 100ms, Cumulative Layout Shift under 0.1, with field data analysis and synthetic monitoring
- Establishes performance baselines before optimization and validates improvements with statistical analysis including confidence intervals and before/after comparisons
- Performs capacity planning with growth forecasting, auto-scaling policy validation, and cost-performance trade-off analysis
- Creates performance budgets enforced in CI/CD pipelines with automated quality gates that block deployments exceeding thresholds
- Produces performance ROI analysis quantifying optimization costs against business impact (conversion rate improvements, infrastructure cost savings)

## Files

| File | Purpose |
|------|---------|
| `SOUL.md` | Performance benchmarker identity, analytical personality, experience with systems succeeding through performance excellence |
| `AGENTS.md` | Performance-first methodology rules, user experience focus requirements, four-step workflow (baseline, testing strategy, analysis, monitoring), and success metrics |
| `SKILL.md` | Complete k6 test suite example with staged load profiles and custom metrics, Core Web Vitals optimization targets, deliverable report template, and advanced capabilities for statistical analysis, caching strategies, and multi-region optimization |

## Quick Start

```bash
cp -r testing-performance-benchmarker/ ~/.openclaw/workspace/
```

## Use Cases

- Running a staged k6 load test from warm-up through 10x peak traffic to find the breaking point and measure recovery behavior
- Optimizing Core Web Vitals for a web application where LCP exceeds 4 seconds, using code splitting, lazy loading, and CDN configuration
- Establishing performance baselines for a new API and creating automated regression tests that fail if p95 response time exceeds 500ms
- Performing capacity planning for a growing SaaS product to forecast when current infrastructure will need scaling and estimate costs
- Producing a performance ROI report showing that a $50K optimization effort reduces server costs by $3,000/month while improving user conversion by 15%
