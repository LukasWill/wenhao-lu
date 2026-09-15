---
title: Causal and Language-Based RL Interpretability
date: 2026-05-28
weight: 1
home_order: 1
summary: Causal representation objectives and language-model probes for explaining and predicting RL-agent behavior from trajectories.
tags:
  - RL interpretability
  - causal analysis
  - mental modeling
featured: true
project_status: Published research · 2 first-author papers
project_contribution: Developed causal state-distillation objectives and evaluated whether language models can form reliable behavioral models from agent interaction histories.
project_methods:
  - Causal representations
  - Trajectory evaluation
  - Language-model probing
project_links:
  - label: TMLR 2025
    url: publications/mental-modeling-rl-agents/
  - label: CLeaR 2024
    url: publications/causal-state-distillation/
links: []
image:
  caption: ""
  focal_point: ""
  preview_only: true
---

**Status:** Publication-backed research spanning two first-author papers.

## Research Question

What evidence is sufficient to explain or predict an RL agent's decisions, and where do common explanation interfaces hide dependencies across state, action, reward, and trajectory history?

## My Contribution

**Causal state distillation.** I developed representation objectives that distill causal factors linking states to actions and reward channels. The method extends reward-decomposition explanations beyond sub-reward attribution and produces compact factors for local explanation.

**Language-model mental modeling.** I studied whether language models can infer an RL agent's behavior and action effects from interaction histories. The evaluation uses explicit behavioral metrics to expose both useful predictions and systematic limitations rather than treating fluent rationales as evidence of understanding.

## Methods

- Causal representation learning with sufficiency, sparsity, and orthogonality objectives.
- Reward-channel and action-factor analysis for local explanations.
- Trajectory-level language-model probes for action and state-transition prediction.

## Evidence

- [Mental Modeling of Reinforcement Learning Agents by Language Models]({{< relref "/publications/mental-modeling-rl-agents" >}}), *Transactions on Machine Learning Research*, 2025.
- [Causal State Distillation for Explainable Reinforcement Learning]({{< relref "/publications/causal-state-distillation" >}}), *Conference on Causal Learning and Reasoning*, 2024 (oral presentation).
