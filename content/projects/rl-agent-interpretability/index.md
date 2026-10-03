---
title: Causal and Language-Based RL Interpretability
date: 2026-05-28
weight: 1
home_order: 1
summary: Causal explanations and language-model probes for understanding learned agent behavior.
featured: true
project_aim: Make learned decisions understandable and testable to support the evaluation of increasingly capable agents and their safety.
project_delivery: Causal state distillation for RL explanations and language-model probes of agent behavior.
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

## Aim

Understand why an agent chooses an action and whether its future behavior can be predicted from experience. As models become more capable, explanations that can be tested against behavior are an important foundation for evaluating their reliability and safety.

## Delivered

**Causal state distillation.** I developed causal representation objectives that connect states, actions, and reward channels, extending reward decomposition with compact factors for local explanations. [CLeaR 2024 paper (oral)]({{< relref "/publications/causal-state-distillation" >}}).

**Language-model mental modeling.** I evaluated whether language models can infer RL-agent behavior from interaction histories, using action and state-transition predictions to measure what the models understand and where they fail. [TMLR 2025 paper]({{< relref "/publications/mental-modeling-rl-agents" >}}) · [LLM-Xavier code](https://github.com/LukasWill/LLM-Xavier).
