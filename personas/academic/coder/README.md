# Coder

Senior ML engineer and experiment scientist within the OpenClaw multi-agent academic system. Transforms research ideas into production-quality code, designs rigorous experiments with reproducibility guarantees, and ensures fair baseline comparisons targeting top-tier AI conferences (ACL, NeurIPS, ICML, ICLR).

## Core Capabilities

- Implements research methods in Python/PyTorch/JAX with HuggingFace Transformers, supporting distributed training via DeepSpeed, FSDP, and Megatron-LM
- Designs and executes rigorous experiment suites including main experiments, ablation studies, case studies, and robustness tests with statistical significance analysis
- Optimizes GPU utilization through mixed precision, gradient checkpointing, efficient attention, and quantization techniques
- Provides systematic debugging methodology for common ML issues (NaN loss, overfitting, OOM, data leakage, metric inconsistency)
- Enforces reproducibility through fixed seeds, config-file management, W&B/MLflow logging, and clean environment documentation
- Generates structured experiment reports with result tables, ablation breakdowns, and findings analysis

## Files

| File | Purpose |
|------|--------|
| `SOUL.md` | ML engineer identity, algorithm implementation, experiment design, coding standards and project structure |
| `AGENTS.md` | Model config, tool access, session management, inter-agent communication protocol |
| `USER.md` | Research domain (AI/NLP/Multi-Agent), target venues, Chinese-primary language preference |

## Quick Start

```bash
cp -r academic-coder/ ~/.openclaw/workspace/
```

## Use Cases

- Scaffold a new ML research project with standardized directory structure, config management, and training pipeline
- Run a full experiment cycle with fair baseline comparisons before a conference deadline
- Debug a training run that produces NaN losses or fails to converge and trace the root cause systematically
- Optimize inference speed and memory usage for a large language model deployment
- Generate a reproducibility-ready codebase with fixed seeds, environment files, and a code review checklist
