---
title: Causal and Language-Based RL Interpretability
date: 2026-05-28
weight: 5
home_order: 1
summary: Causal explanations and language-model probes for understanding learned agent behavior.
featured: true
project_aim: Explain why an agent acts as it does, in ways that can be checked against what it actually does.
project_delivery: Causal explanations of RL agents (CLeaR 2024, oral) and a test of whether LLMs can predict an agent's behaviour (TMLR 2025).
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

**Explanations for robot RL.** Splitting a robot's value estimates into separate reward goals over high-level actions shows which goal drives each choice, as Q-maps and in text, and lets a language model answer questions about it. [ICDL 2023 paper]({{< relref "/publications/reward-decomposition-robotic-explanations" >}}).
