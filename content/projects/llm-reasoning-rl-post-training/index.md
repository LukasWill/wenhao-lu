---
title: LLM Reasoning and RL Post-Training
date: 2026-07-01
weight: 2
home_order: 2
summary: Better language-model reasoning and alignment through curriculum-based AI feedback and logic-guided chain-of-thought refinement.
featured: true
project_aim: Improve LLM reasoning and alignment through RL post-training and explicit checks on reasoning steps.
project_delivery: Curriculum-RLAIF for preference learning and Logical Thoughts for logic-guided chain-of-thought revision.
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
