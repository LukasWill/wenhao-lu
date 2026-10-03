---
title: RL for Obstacle-Aware Robotic Manipulation
date: 2026-05-28
weight: 5
summary: Reward and observation design for obstacle-aware manipulation, now part of the robot learning and VLA failure prediction thread.
featured: false
build:
  list: never
project_aim: Learn long-horizon manipulation policies that account for obstacles and changing subgoals.
project_direction: Ongoing simulation work on reward design, distance-field observations, and trajectory evaluation.
project_links:
  - label: Robot learning thread
    url: projects/failure-aware-vla-inference/
links: []
image:
  caption: ""
  focal_point: ""
  preview_only: true
---

This work is now part of [Robot Learning and VLA Failure Prediction]({{< relref "/projects/failure-aware-vla-inference" >}}).

I am developing reward and observation designs for long-horizon, obstacle-aware manipulation in simulation. Gaussian Process Distance Fields provide continuous obstacle-distance and gradient signals; evaluation separates task completion from collisions, path quality, and subgoal progress. Public results are forthcoming.
