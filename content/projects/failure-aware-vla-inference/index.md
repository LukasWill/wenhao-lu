---
title: Failure-Aware Fast Inference for VLA-Style Models
date: 2026-06-13
summary: An ongoing project using failure detection modules to support faster, safer inference and exploring their use as efficient supervision for VLA fine-tuning.
tags:
  - robot foundation models
  - VLA
  - failure detection
  - efficient inference
  - embodied AI
featured: true
links: []
image:
  caption: "TODO: add representative project image."
  focal_point: ""
  preview_only: true
---

This ongoing project studies failure detection modules as general plug-ins for VLA-style robot foundation models. The working goal is to use detected failure risk to allocate inference-time computation and potentially provide an efficient supervisory signal for fine-tuning.

## Motivation

VLA-style models can be expensive to query repeatedly during long-horizon embodied tasks. A lightweight detector may help decide when an action can follow a fast path, when additional inference or reconsideration is warranted, and which trajectories provide useful corrective supervision.

## Project Direction

- Failure detection as a modular add-on rather than a model-specific redesign.
- Faster and safer execution through risk-aware routing, selective querying, or early rejection.
- Potential use of failure signals as targeted supervision for efficient VLA fine-tuning.
- Joint evaluation of latency, compute, calibration, failure rate, and task success.

## Relation to Prior Work

- [SAFE](https://openreview.net/forum?id=XPyAukgsFf) is the closest detector-centric baseline: it predicts failure from internal features of multiple VLA families. Our focus extends beyond transferable detection to using the detector for compute allocation and fine-tuning supervision.
- [FPC-VLA](https://arxiv.org/abs/2509.04018) places a VLM-based supervisor in the control loop to predict failures and propose corrections. Our target is a lighter, general plug-in for inference routing and learning signals, rather than a correction-generating dual-model framework.
- [ReconVLA](https://arxiv.org/abs/2604.16677) uses conformal uncertainty over actions and robot states for proactive risk detection and action selection. We instead center explicit failure signals and their dual use at inference and during fine-tuning.
- [Temporal Difference Calibration](https://arxiv.org/abs/2604.20472) estimates calibrated success confidence along partial trajectories and connects it to value estimation. Our focus is modular failure detection as a systems mechanism, not calibration as the primary objective.
- [DreamAvoid](https://arxiv.org/abs/2605.11750) triggers world-model rollouts during critical phases to rank candidate actions. Our approach aims to avoid routine expensive reasoning through lightweight detection, without requiring test-time future simulation.
- [WMPO](https://arxiv.org/abs/2511.09515) optimizes VLA policies with imagined trajectories and success/failure rewards. It informs our fine-tuning direction, but our core object is the reusable failure detector rather than world-model-based policy optimization.
- [FARL](https://arxiv.org/abs/2601.07821) combines a world-model safety critic with recovery for safer offline-to-online RL. It is not VLA-specific and emphasizes safe exploration and recovery; we emphasize VLA inference efficiency and detector-guided fine-tuning.

## Preliminary Results and Videos

Preliminary results, rollout videos, and qualitative comparisons will be added here once experiments are ready.

<!--
Future videos can be placed under:
static/uploads/projects/failure-aware-vla-inference/

Example future embed:
<video controls preload="metadata" class="w-full rounded-lg">
  <source src="/uploads/projects/failure-aware-vla-inference/example-rollout.mp4" type="video/mp4">
</video>
-->

## Links

- TODO: add paper or manuscript link when available.
- TODO: add code link when available.
- TODO: add demo videos and preliminary results.

## References

- Qiao Gu et al. "SAFE: Multitask Failure Detection for Vision-Language-Action Models." *Advances in Neural Information Processing Systems (NeurIPS)*, 2025. [OpenReview](https://openreview.net/forum?id=XPyAukgsFf).
- Yifan Yang et al. "FPC-VLA: A Vision-Language-Action Framework with a Supervisor for Failure Prediction and Correction." arXiv:2509.04018, 2025. [arXiv](https://arxiv.org/abs/2509.04018).
- Lingling Chen, Zongyao Lyu, and William J. Beksi. "ReconVLA: An Uncertainty-Guided and Failure-Aware Vision-Language-Action Framework for Robotic Control." arXiv:2604.16677, 2026. [arXiv](https://arxiv.org/abs/2604.16677).
- Shelly Francis-Meretzki, Mirco Mutti, Yaniv Romano, and Aviv Tamar. "Temporal Difference Calibration in Sequential Tasks: Application to Vision-Language-Action Models." arXiv:2604.20472, 2026. [arXiv](https://arxiv.org/abs/2604.20472).
- Xianzhe Fan et al. "DreamAvoid: Critical-Phase Test-Time Dreaming to Avoid Failures in VLA Policies." arXiv:2605.11750, 2026. [arXiv](https://arxiv.org/abs/2605.11750).
- Fangqi Zhu, Zhengyang Yan, Zicong Hong, Quanxin Shou, Xiao Ma, and Song Guo. "WMPO: World Model-based Policy Optimization for Vision-Language-Action Models." arXiv:2511.09515, 2025. [arXiv](https://arxiv.org/abs/2511.09515).
- Huanyu Li et al. "Failure-Aware RL: Reliable Offline-to-Online Reinforcement Learning with Self-Recovery for Real-World Manipulation." arXiv:2601.07821, 2026. [arXiv](https://arxiv.org/abs/2601.07821).
