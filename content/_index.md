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
        I am a PhD researcher in robot learning and AI. My work focuses on
        reinforcement learning for robotic manipulation and on interpretability
        methods that make RL agents easier to analyze, explain, and trust.
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
        size: large
        shape: rounded

  - block: markdown
    id: themes
    content:
      title: Research Themes
      subtitle: ''
      text: |-
        My research centers on two anchors: RL-driven robot learning and interpretability for RL agents. I study how learned agents acquire useful behavior in robotic tasks, and how their decisions can be analyzed beyond aggregate reward.

        <div class="grid gap-6 md:grid-cols-3 not-prose">
          <div class="rounded-lg border border-gray-200 dark:border-gray-700 p-6">
            <h3 class="mt-0 text-lg font-semibold">RL-Driven Robot Learning</h3>
            <p>I study reinforcement learning for robotic manipulation and embodied control, with an emphasis on reward design, obstacle-aware behavior, and learning from interaction.</p>
          </div>
          <div class="rounded-lg border border-gray-200 dark:border-gray-700 p-6">
            <h3 class="mt-0 text-lg font-semibold">Interpretable RL Agents</h3>
            <p>I develop methods and evaluations for understanding why RL agents act, including reward decomposition, causal state distillation, action coherence, and trajectory-level explanations.</p>
          </div>
          <div class="rounded-lg border border-gray-200 dark:border-gray-700 p-6">
            <h3 class="mt-0 text-lg font-semibold">Foundation Models for RL Explanations</h3>
            <p>I use language and vision-language models as tools for querying, summarizing, and stress testing explanations, while keeping the learned RL policy as the central object of study.</p>
          </div>
        </div>
    design:
      columns: '1'

  - block: collection
    id: projects
    content:
      title: Selected Projects
      text: Three project threads that summarize my research trajectory.
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
      text: Selected first-author work most closely aligned with RL-driven robot learning and interpretability for RL agents.
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
        My long-term goal is to develop RL-driven robotic systems whose behavior can be improved, inspected, and explained. I am especially interested in the connection between reinforcement learning, embodied interaction, and interpretability: agents should not only complete tasks, but also expose reliable evidence about why they act.
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
        **Current:** PhD Researcher, University of Hamburg.

        **Research areas:** reinforcement learning, robot learning, robotic manipulation, and interpretability for RL agents.
    design:
      columns: '1'

  - block: markdown
    id: technical
    content:
      title: Technical Capabilities
      text: |-
        **Reinforcement Learning:** PPO, reward shaping, reward decomposition, trajectory-level evaluation.

        **Robot Learning:** robotic manipulation, simulation-based learning, obstacle-aware behavior, embodied control.

        **Interpretability:** causal state distillation, high-level robotic explanations, mental modeling of RL agents, action coherence analysis.
    design:
      columns: '1'

  - block: markdown
    id: contact
    content:
      title: Contact
      text: |-
        I am open to research discussions and collaborations related to robot learning, reinforcement learning, and interpretable RL-agent behavior.

        Email: [wenhao.lu@uni-hamburg.de](mailto:wenhao.lu@uni-hamburg.de)
    design:
      columns: '1'
---
