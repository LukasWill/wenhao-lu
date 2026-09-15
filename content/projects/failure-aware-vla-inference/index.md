---
title: Failure-Aware Fast Inference for VLA-Style Models
date: 2026-06-13
weight: 2
home_order: 2
summary: A modular failure-detection layer for allocating VLA inference compute and identifying trajectory segments for corrective fine-tuning.
tags:
  - robot foundation models
  - VLA
  - failure detection
  - efficient inference
  - embodied AI
featured: true
project_status: Ongoing research · Public results forthcoming
project_contribution: Developing a model-agnostic failure detector that routes inference compute and identifies high-risk transitions for targeted fine-tuning.
project_methods:
  - Failure detection
  - Selective inference
  - Detector calibration
project_links: []
links: []
image:
  caption: ""
  focal_point: ""
  preview_only: true
---

**Status:** Ongoing research. Quantitative results, code, and rollout media will be added only after they are ready for public release.

## Problem

VLA-style robot policies normally pay a similar inference cost at every step even though some transitions are routine and others are precursors to failure. A useful failure signal should identify those differences without requiring every base policy to be redesigned.

## What I Am Developing

- A lightweight, model-agnostic detector that estimates failure risk across VLA families.
- An inference-routing policy that uses calibrated risk to choose a fast path, request additional computation, or reject an unsafe continuation.
- A fine-tuning signal that prioritizes high-risk transitions and failure precursors rather than treating all collected trajectory segments uniformly.

## Evaluation

The release criteria go beyond task success. The planned comparison measures latency, inference compute, detector calibration, false-negative failures, intervention frequency, and end-to-end success. Ablations will separate the detector, routing policy, and detector-guided fine-tuning.

## Public Evidence

No project-specific result is claimed yet. The closest detector-centric baseline is [SAFE](https://openreview.net/forum?id=XPyAukgsFf), which predicts VLA failures from internal features. [FPC-VLA](https://arxiv.org/abs/2509.04018) uses a VLM supervisor for failure prediction and correction, while [Temporal Difference Calibration](https://arxiv.org/abs/2604.20472) estimates calibrated success confidence along partial trajectories. This project instead centers a lightweight reusable detector and its dual role in inference routing and fine-tuning.
