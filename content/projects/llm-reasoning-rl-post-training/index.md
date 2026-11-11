---
title: LLM Reasoning and RL Post-Training
date: 2026-07-01
weight: 4
home_order: 2
summary: Better language-model reasoning and alignment through curriculum-based AI feedback and logic-guided chain-of-thought refinement.
featured: true
project_aim: Make LLMs reason better, both by training them with RL from AI feedback and by checking their reasoning step by step.
project_delivery: Curriculum-RLAIF (ACL Findings 2026), which trains reward models from easy to hard examples, and Logical Thoughts (LREC-COLING 2024), which checks chain-of-thought steps with logic.
project_links:
  - label: Curriculum-RLAIF
    url: publications/curriculum-rlaif/
  - label: Logical Thoughts
    url: publications/logic-thoughts-lrec-coling/
links: []
image:
  caption: ""
  focal_point: ""
  preview_only: true
---

## Aim

Make language models better at following feedback and solving multi-step problems. This thread brings together RL post-training from AI feedback and explicit verification of chain-of-thought reasoning.

## Delivered

**Curriculum-RLAIF.** Our work trains reward models on preference pairs ordered by difficulty, improving reward-model generalization and downstream policy alignment. It connects curriculum learning with reinforcement learning from AI feedback. [ACL Findings 2026 paper and code]({{< relref "/publications/curriculum-rlaif" >}}).

**Logical Thoughts.** Our prompting framework uses symbolic-logic principles to verify and revise zero-shot chain-of-thought steps across multi-step tasks. It complements training-based alignment with reasoning checks at inference time. [LREC-COLING 2024 paper]({{< relref "/publications/logic-thoughts-lrec-coling" >}}).
