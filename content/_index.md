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
        I am a PhD researcher working at the intersection of reinforcement
        learning, interpretability, and foundation models for robot learning. My
        research develops and analyzes RL-driven embodied agents, with a focus on
        robotic manipulation, agent reliability, and explanations that make
        learned behavior easier to inspect and trust.
      headings:
        about: About Me
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

  - block: collection
    id: papers
    content:
      title: Featured Publications
      text: Selected papers and coauthored work, ordered newest first.
      filters:
        folders:
          - publications
      order: desc
      count: 20
    design:
      view: citation
      columns: 1

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
    id: activities
    content:
      title: Professional Activities
      text: |-
        **Conference Reviewer:** AISTATS 2025, NeurIPS 2025, NeurIPS 2024.
    design:
      columns: '1'

  - block: markdown
    id: contact
    content:
      title: Contact
      text: |-
        I am open to research discussions and collaborations on RL-driven robot learning, interpretability for understanding foundation-model behavior, and the synergy between reinforcement learning and foundation models. I am especially interested in RL for robot foundation models in embodied scenarios.

        Email: [wenhao.lu@uni-hamburg.de](mailto:wenhao.lu@uni-hamburg.de)
    design:
      columns: '1'
---
