---
title: ''
summary: ''
date: 2026-05-28
type: landing

sections:
  - block: resume-biography-3
    id: about
    content:
      username: me
      text: >-
        I am a PhD researcher in robot learning and AI. My work studies
        reinforcement learning for embodied and agentic decision-making systems,
        with a focus on robotic manipulation, long-horizon tasks, reliable
        LLM/VLM agents, and interpretable behavior.
      button:
        text: Download CV
        url: uploads/resume.pdf
      headings:
        about: ''
        education: ''
        interests: ''
    design:
      background:
        gradient_mesh:
          enable: true
      name:
        size: md
      avatar:
        size: medium
        shape: circle

  - block: markdown
    id: themes
    content:
      title: Research Themes
      subtitle: ''
      text: |-
        My research studies how reinforcement learning can produce capable, reliable, and interpretable decision-making agents. I work across robot learning, long-horizon manipulation, LLM/VLM agents, and RL-based post-training, with a particular interest in when task success does or does not imply reliable reasoning or behavior.

        <div class="grid gap-6 md:grid-cols-2 not-prose">
          <div class="rounded-lg border border-gray-200 dark:border-gray-700 p-6">
            <h3 class="mt-0 text-lg font-semibold">Robot Learning & Manipulation</h3>
            <p>I study reinforcement learning methods for robotic manipulation and embodied control, with an emphasis on long-horizon tasks, obstacle-aware behavior, and sample-efficient learning.</p>
          </div>
          <div class="rounded-lg border border-gray-200 dark:border-gray-700 p-6">
            <h3 class="mt-0 text-lg font-semibold">Reinforcement Learning for Long-Horizon Decision Making</h3>
            <p>I am interested in agents that must plan, act, and adapt over multiple turns or subgoals, including task decomposition, reward design, and evaluation of multi-turn behavior.</p>
          </div>
          <div class="rounded-lg border border-gray-200 dark:border-gray-700 p-6">
            <h3 class="mt-0 text-lg font-semibold">Reliable LLM/VLM Agents</h3>
            <p>I investigate how RL-based post-training changes the behavior of language and vision-language agents, especially whether task success is accompanied by reliable reasoning traces.</p>
          </div>
          <div class="rounded-lg border border-gray-200 dark:border-gray-700 p-6">
            <h3 class="mt-0 text-lg font-semibold">Explainability & Interpretability</h3>
            <p>I develop analyses and evaluation protocols for understanding learned agents, including reasoning trace reliability, action coherence, grounding, temporal consistency, and mechanistic diagnostics.</p>
          </div>
        </div>
    design:
      columns: '1'

  - block: collection
    id: projects
    content:
      title: Selected Projects
      text: Representative project areas connecting robotics/RL with interpretable and reliable agent behavior.
      filters:
        folders:
          - projects
        featured_only: true
    design:
      view: article-grid
      columns: 2
      fill_image: false
      show_date: false
      show_read_time: false
      show_read_more: false

  - block: collection
    id: papers
    content:
      title: Featured Publications
      text: Selected work most closely aligned with RL-driven robot learning and interpretability for RL agents.
      filters:
        folders:
          - publications
        featured_only: true
    design:
      view: citation
      columns: 1

  - block: markdown
    id: vision
    content:
      title: Research Vision
      text: |-
        My long-term goal is to develop learning-based robotic and agentic systems that are not only successful in task execution, but also robust, inspectable, and trustworthy. I am especially interested in connecting reinforcement learning, foundation models, and embodied interaction, where agents must act over long horizons while maintaining reliable internal and external behavior.
    design:
      columns: '1'

  - block: collection
    id: news
    content:
      title: News
      page_type: blog
      count: 4
      filters:
        author: ''
        category: ''
        tag: ''
        exclude_featured: false
        exclude_future: false
        exclude_past: false
        publication_type: ''
      order: desc
    design:
      view: date-title-summary
      spacing:
        padding: [0, 0, 0, 0]

  - block: markdown
    id: cv
    content:
      title: Experience / CV
      text: |-
        **Current:** PhD Researcher, University of Hamburg. Lab affiliation details should be finalized before publishing this staging site.

        **Education:** PhD Researcher in robot learning, reinforcement learning, and explainable AI at the University of Hamburg.

        **Research areas:** reinforcement learning, robot learning, robotic manipulation, LLM/VLM agents, RL post-training, and interpretability.

        Note: the downloadable CV file exists in this staging repo and should be verified before publication.
    design:
      columns: '1'

  - block: markdown
    id: technical
    content:
      title: Technical Capabilities
      text: |-
        **Reinforcement Learning:** PPO, reward shaping, reward decomposition, long-horizon decision making, trajectory-level evaluation.

        **Robot Learning:** robotic manipulation, simulation-based learning, obstacle-aware behavior, task decomposition, embodied control.

        **Foundation Models:** LLM/VLM agents, reasoning traces, RL-based post-training, LLM-as-judge evaluation, multimodal agent evaluation.

        **Engineering Tools:** PyTorch, robotics simulation, experiment analysis. Additional infrastructure tools should be added only after verification.
    design:
      columns: '1'

  - block: markdown
    id: contact
    content:
      title: Contact
      text: |-
        I am open to research discussions and collaborations related to robot learning, reinforcement learning, reliable LLM/VLM agents, and embodied AI.

        Email: [wenhao.lu@uni-hamburg.de](mailto:wenhao.lu@uni-hamburg.de)
    design:
      columns: '1'
---
