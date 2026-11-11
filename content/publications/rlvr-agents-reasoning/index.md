---
title: "RLVR Makes Agents Win More, but Not Necessarily Reason Better"
authors:
  - me
  - Jae Hee Lee
  - Josua Spisak
  - Xufeng Zhao
  - Stefan Wermter
date: "2026-11-01T00:00:00Z"
publishDate: "2026-11-01T00:00:00Z"
publication:
  name: "NeurIPS 2026 Workshops: Interpreting Agent Behavior (IAB) and Evaluation of Interactive Agents"
  short_name: "NeurIPS 2026 Workshops"
summary: "RL training makes LLM/VLM agents win far more often (ALFWorld: 8.6% to 85.2%), but the runs that win reason barely better than the runs that lose."
featured: true
tags:
  - reinforcement learning
  - RLVR
  - LLM agents
  - VLM agents
  - reasoning reliability
paper_links:
  - type: source
    url: https://openreview.net/forum?id=jsTJu11CIh
    label: OpenReview (IAB)
  - type: source
    url: https://openreview.net/forum?id=xpTzSAVfAF
    label: OpenReview (EIA)
  - type: code
    url: https://github.com/LukasWill/tracerigor
    label: Code
image:
  preview_only: true
---

**TL;DR:** Five agents (Qwen2.5-3B/7B and Qwen2.5-VL-3B) are trained with multi-turn PPO on ALFWorld, ScienceWorld, Sokoban, and AI2-THOR Navigation, and every evaluation turn is judged for observation grounding, action coherence, and temporal consistency. Task performance rises sharply (ALFWorld success climbs from 8.6% to 85.2%). Within a checkpoint, however, a randomly drawn high performer is more reliable than a low performer only 55–70% of the time, where 50% is chance.

{{< publication_links >}}

## BibTeX

```bibtex
@inproceedings{lu2026rlvr,
  title = {{RLVR} Makes Agents Win More, but Not Necessarily Reason Better},
  author = {Lu, Wenhao and Lee, Jae Hee and Spisak, Josua and Zhao, Xufeng and Wermter, Stefan},
  booktitle = {The 1st Workshop on Interpreting Agent Behavior (IAB) at NeurIPS 2026},
  year = {2026},
  url = {https://openreview.net/forum?id=jsTJu11CIh}
}
```
