---
title: Robot Learning and VLA Failure Prediction
date: 2026-06-13
weight: 3
home_order: 3
summary: Robot training and planning across RL, VLMs, and VLAs, with a focus on predicting failures before they unfold.
featured: true
project_aim: Predict VLA failures and improve robot learning through reward, observation, and inference design.
project_delivery: Directional VLM rewards for sample-efficient robot RL and LLM/VLM task planning.
project_links:
  - label: VLM rewards
    url: publications/directional-vlm-rewards/
  - label: Bimanual planning
    url: publications/llms-orchestrating-bimanual-robots/
links: []
image:
  caption: ""
  focal_point: ""
  preview_only: true
---

## Aim

Build robot policies that can complete long-horizon tasks while recognizing when a trajectory is likely to fail. This thread connects reinforcement learning, vision-language reasoning, and vision-language-action policies through training signals, planning, and failure prediction.

## Delivered

**VLM rewards for robot RL.** Our directional reward combines a VLM's assessment of the current state with whether recent visual changes move toward the goal. Evaluated on six MetaWorld manipulation tasks, it improves exploration and sample efficiency. [SII 2026 paper]({{< relref "/publications/directional-vlm-rewards" >}}) · [Code](https://github.com/LukasWill/directional_vlm_rl).

**LLM/VLM robot planning.** My coauthored work on [bimanual robot orchestration]({{< relref "/publications/llms-orchestrating-bimanual-robots" >}}) uses an LLM to coordinate long-horizon manipulation in simulation. Our [object-state-sensitive planning work]({{< relref "/publications/object-state-sensitive-task-planning" >}}) studies LLM/VLM agents and introduces a multimodal tabletop benchmark for state-aware planning.

## Current Work

**VLA failure prediction.** I am developing a lightweight detector to identify failure precursors, allocate inference computation where it is needed, and select trajectory segments for corrective fine-tuning. Evaluation targets failure detection, calibration, latency, and task success.

**RL manipulation.** I am designing rewards and observations for obstacle-aware manipulation, including Gaussian Process Distance Fields that expose obstacle distances and gradients. Simulation studies examine collisions, path quality, and subgoal progress alongside task completion.

The VLA detector and obstacle-aware manipulation experiments are ongoing and have not yet been released publicly.
