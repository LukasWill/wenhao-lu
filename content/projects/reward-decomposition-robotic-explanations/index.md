---
title: Reward Decomposition for Robotic Explanations
date: 2026-05-28
weight: 6
summary: High-level explanations of RL-driven robot behavior using decomposed action values, abstract actions, and task-level object properties.
featured: false
build:
  list: never
project_aim: Explain the reward trade-offs and future consequences behind a robot's actions.
project_delivery: An explanation layer combining decomposed action values, abstract actions, and object-level task properties.
project_links:
  - label: ICDL 2023 paper
    url: publications/reward-decomposition-robotic-explanations/
links: []
image:
  caption: ""
  focal_point: ""
  preview_only: true
---

## Problem

A scalar return hides the trade-offs behind an action, while one-step explanations can miss consequences that unfold later in a trajectory. Low-level robotic state and action spaces make both problems difficult to communicate directly.

## Contribution

- An explainable Q-map framework that combines decomposed action values with abstract, task-specific actions.
- Visual and textual explanations grounded in object properties and future reward components.
- Quantitative and qualitative analysis in two robotic scenarios, plus a language model that answers questions about the explanations.

## Evidence

[A Closer Look at Reward Decomposition for High-Level Robotic Explanations]({{< relref "/publications/reward-decomposition-robotic-explanations" >}}), *IEEE International Conference on Development and Learning*, 2023.
