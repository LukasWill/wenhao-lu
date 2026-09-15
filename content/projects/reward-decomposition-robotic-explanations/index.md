---
title: Reward Decomposition for Robotic Explanations
date: 2026-05-28
weight: 4
summary: High-level explanations of RL-driven robot behavior using decomposed action values, abstract actions, and task-level object properties.
tags:
  - explainable RL
  - reward decomposition
  - robotics
featured: false
project_status: Published research · ICDL 2023 oral
project_contribution: Developed and evaluated an explanation layer combining decomposed action values with abstract actions and object-level task properties.
project_methods:
  - Reward decomposition
  - Explainable Q-maps
  - Robotic evaluation
project_links:
  - label: ICDL 2023 paper
    url: publications/reward-decomposition-robotic-explanations/
links: []
image:
  caption: ""
  focal_point: ""
  preview_only: true
---

**Status:** Publication-backed work presented orally at ICDL 2023.

## Problem

A scalar return hides the trade-offs behind an action, while one-step explanations can miss consequences that unfold later in a trajectory. Low-level robotic state and action spaces make both problems difficult to communicate directly.

## Contribution

- An explainable Q-map framework that combines decomposed action values with abstract, task-specific actions.
- Visual and textual explanations grounded in object properties and future reward components.
- Quantitative and qualitative analysis in two robotic scenarios, including exploratory integration of explanation artifacts with language models.

The contribution is the explanation layer. The robotic scenarios provide embodied evaluation settings; this work does not claim a new manipulation controller or obstacle-avoidance method.

## Evidence

[A Closer Look at Reward Decomposition for High-Level Robotic Explanations]({{< relref "/publications/reward-decomposition-robotic-explanations" >}}), *IEEE International Conference on Development and Learning*, 2023.
