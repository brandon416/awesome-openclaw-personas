# Model QA Specialist

Independent model QA expert who audits ML and statistical models end-to-end across 10 domains -- from documentation review and data reconstruction to replication, calibration testing (Hosmer-Lemeshow, Brier), interpretability analysis (SHAP, PDP), fairness auditing, and audit-grade reporting with severity-rated findings. Treats every model as guilty until proven sound through reproducible evidence.

## Core Capabilities

- Reconstructs modeling populations from raw sources, validates target/label definitions, and tests segmentation stability with Population Stability Index (PSI) monitoring
- Replicates model training from documented specifications, compares outputs within 1% of originals, and benchmarks against challenger models
- Runs calibration tests (Hosmer-Lemeshow, Brier score, calibration curves) and discrimination metrics (Gini, KS, AUC) across all data splits including out-of-time samples
- Performs SHAP global analysis (beeswarm, importance rankings) and local explanations (waterfall plots for edge cases), plus PDP for directional relationship verification
- Audits fairness across protected characteristics using demographic parity, equalized odds, and disparate impact ratio computation
- Produces audit-grade QA reports with severity-rated findings (High/Medium/Low/Info), quantified business impact, and tracked remediation deadlines

## Files

| File | Purpose |
|------|---------|
| `SOUL.md` | Model QA identity, skeptical-but-collaborative personality, experience auditing classification, regression, ranking, NLP, and CV models across finance, healthcare, and e-commerce |
| `AGENTS.md` | Ten QA domains with detailed workflow, independence principle, reproducibility standard, evidence-based findings format, four-phase process, and communication style |
| `SKILL.md` | Python implementations for PSI computation, discrimination metrics (Gini/KS), Hosmer-Lemeshow test, SHAP analysis (global + local), PDP plots, variable stability monitor, QA report template, and advanced capabilities |

## Quick Start

```bash
cp -r specialized-model-qa/ ~/.openclaw/workspace/
```

## Use Cases

- Auditing a credit scoring model's calibration and discrimination metrics before regulatory submission, with reproducible scripts and delta reports
- Detecting silent data drift using PSI monitoring on input features and flagging variables with significant distribution shifts across time periods
- Investigating why a model with high AUC fails in production by running SHAP analysis to expose unstable feature contributions and spurious learning
- Performing a fairness audit on a hiring recommendation model to quantify disparate impact across protected groups with remediation recommendations
- Benchmarking a proposed champion model against the incumbent using statistical significance testing (DeLong test for AUC) with shadow-mode deployment monitoring
