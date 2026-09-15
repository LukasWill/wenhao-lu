---
title: Reasoning Reliability under RL Fine-Tuning
date: 2026-05-28
summary: We study whether RL fine-tuning improves not only task success but also
  the reliability of visible reasoning traces in multi-turn LLM/VLM agents. The
  analysis separates aggregate reward-quality co-movement from within-checkpoint
  trajectory-level coupling.
tags:
  - RLFT
  - RLVR
  - LLM agents
  - VLM agents
  - reasoning reliability
  - interpretability
featured: false
draft: true
build:
  render: never
  list: never
links: []
image:
  caption: "TODO: add representative analysis figure."
  focal_point: ""
  preview_only: true

---

We study whether RL fine-tuning improves not only task success but also the reliability of visible reasoning traces in multi-turn LLM/VLM agents. The analysis separates aggregate reward-quality co-movement from within-checkpoint trajectory-level coupling.

## Motivation

Higher task reward does not automatically imply reliable reasoning. This project asks when RL-based post-training improves visible reasoning traces and when success and reasoning quality decouple.

## What I Worked On

- Evaluation of multi-turn LLM/VLM agents under RL fine-tuning.
- Separation of aggregate reward-quality co-movement from trajectory-level coupling.
- Reliability analysis for reasoning traces, action coherence, and long-horizon behavior.

## Representative Outputs

- TODO: add official paper title.
- TODO: verify public manuscript status before listing this as submitted, under review, or accepted.

## Links

- TODO: add paper link.
- TODO: add code link if public.
- TODO: add dataset or evaluation link if public.

## Research Context

- [DeepSeek-R1](https://arxiv.org/abs/2501.12948) demonstrates how large-scale RL can elicit stronger reasoning behavior. This project asks the separate question of whether higher task reward is accompanied by more reliable visible reasoning.
- [Scaling Laws for Reward Model Overoptimization](https://proceedings.mlr.press/v202/gao23h.html) shows that optimizing a proxy reward can eventually reduce performance under a stronger reference measure. It motivates separating reward trends from independent quality judgments.
- [Language Models Don't Always Say What They Think](https://proceedings.neurips.cc/paper_files/paper/2023/hash/ed3fea9033a80fea1376299fa7863f4a-Abstract.html) demonstrates that plausible chains of thought can omit causal influences on an answer. This project extends the reliability question to multi-turn, RL-fine-tuned agent trajectories.
- [Reasoning Models Don't Always Say What They Think](https://www.anthropic.com/research/reasoning-models-dont-say-think) studies chain-of-thought faithfulness in reasoning models, including after training against exploitable rewards. Our focus is checkpoint- and trajectory-level coupling between task reward and reasoning quality.

## References

- DeepSeek-AI et al. "DeepSeek-R1: Incentivizing Reasoning Capability in LLMs via Reinforcement Learning." 2025. [arXiv](https://arxiv.org/abs/2501.12948).
- Leo Gao, John Schulman, and Jacob Hilton. "Scaling Laws for Reward Model Overoptimization." *ICML*, 2023. [Proceedings](https://proceedings.mlr.press/v202/gao23h.html).
- Miles Turpin, Julian Michael, Ethan Perez, and Samuel Bowman. "Language Models Don't Always Say What They Think: Unfaithful Explanations in Chain-of-Thought Prompting." *NeurIPS*, 2023. [Proceedings](https://proceedings.neurips.cc/paper_files/paper/2023/hash/ed3fea9033a80fea1376299fa7863f4a-Abstract.html).
- Yanda Chen et al. "Reasoning Models Don't Always Say What They Think." 2025. [Research page](https://www.anthropic.com/research/reasoning-models-dont-say-think).
