---
title: RL for Obstacle-Aware Robotic Manipulation
date: 2026-05-28
weight: 3
home_order: 3
summary: Reward and observation design for long-horizon manipulation under geometric constraints, evaluated beyond task success alone.
tags:
  - robot learning
  - reinforcement learning
  - manipulation
featured: true
project_status: Ongoing research · Simulation studies
project_contribution: Designing GPDF-based reward and observation signals, with diagnostics for completion, collision behavior, path quality, and subgoal progression.
project_methods:
  - Reward shaping
  - GPDF representations
  - Simulation evaluation
project_links: []
links: []
image:
  caption: ""
  focal_point: ""
  preview_only: true
---

**Status:** Ongoing simulation research. Public manipulation results will be added when the corresponding experiments are ready for release.

## Problem

Long-horizon manipulation policies must make coherent decisions under geometric constraints, delayed task feedback, and changing subgoals. Final success alone does not show whether a policy learned safe, efficient behavior or reached the goal through brittle trajectories.

## What I Am Developing

- Reward and observation designs that expose task progress and obstacle proximity to a manipulation policy.
- Gaussian Process Distance Field representations that provide continuous distance and gradient information around obstacles.
- Evaluation diagnostics that separate task completion from collision behavior, path quality, and subgoal progression.

## Technical Scope

The current work focuses on controlled simulation studies of policy learning. It does not claim QT-Opt-scale data, real-robot deployment, or public VLA adaptation results.

## Related Published Work

My coauthored work on [bimanual robot orchestration]({{< relref "/publications/llms-orchestrating-bimanual-robots" >}}) and [object state-sensitive task planning]({{< relref "/publications/object-state-sensitive-task-planning" >}}) provides planning context for this direction. Those papers are not presented as validation of the RL manipulation methods described here.
