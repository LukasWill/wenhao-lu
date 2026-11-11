---
title: 'RL Post-Training, Agents & Robot Learning'
summary: 'Wenhao Lu trains LLM/VLM agents and robot policies with reinforcement learning, and measures whether higher reward means better behaviour.'
date: 2026-08-14
type: landing
image:
  filename: authors/me.jpg

sections:
  - block: portfolio-hero
    id: home
    content:
      eyebrow: Research Associate & PhD Researcher · University of Hamburg
      title: Wenhao Lu
      positioning: Interpretable agents, stronger reasoning, reliable robots.
      text: >-
        I study how RL agents make decisions and how to improve them. My work spans
        causal interpretability, LLM reasoning and RL post-training, and robot learning
        with foundation models that are aware of the consequences of their actions,
        such as knowing when they are about to fail.
      availability: Open to research-engineer roles in RL post-training, VLAs and world models, and embodied AI.
      actions:
        - text: See selected work
          url: '#work'
          style: primary
        - text: GitHub
          url: https://github.com/LukasWill
          style: text
        - text: Google Scholar
          url: 'https://scholar.google.com/citations?user=YZt2J_YAAAAJ&hl=de&oi=ao'
          style: text
      image_alt: Wenhao Lu
    design:
      css_class: portfolio-hero-section
      spacing:
        padding: [0, 0, 0, 0]

  # Media-first case studies. Item schema: layouts/_partials/hbx/blocks/portfolio-showcase/block.html
  # and layouts/_partials/showcase/card.html. Videos live under static/, images under assets/.
  - block: portfolio-showcase
    id: work
    content:
      eyebrow: Selected work
      title: From human demonstrations to robot behaviour
      compact_title: Robot learning and collaborations
      items:
        - size: feature
          media: left
          title: 'phone2panda: robot policies from phone videos of my hand'
          summary: >-
            I filmed my own hand putting a bowl on a plate with an iPhone, and turned ten
            of those recordings into a Franka Panda policy in simulation, with no
            teleoperation.
          points:
            - '**What I did.** Each recording becomes a metric 3D demonstration (LiDAR, camera pose, printed tags), is retargeted to the robot''s scene, and is multiplied into 438 simulator-verified robot demos. An ACT policy learns from them; offline RL and a world model are tested on top.'
            - '**Result.** The policy succeeds 98% of the time in scenes it never trained in, as often as one trained on 49 teleoperated demos (97%). Copying my whole hand motion gives only 57%.'
            - '**Takeaway.** Transfer the contact, not the path: where the hand grasps, how it carries, and where it sets down. The robot should plan its own free motion instead of copying mine.'
          gallery:
            - image: media/portfolio/phone2panda-phone-strip.jpg
              caption: One of my iPhone recordings (background blurred). Tags on the table, bowl, and plate give a metric frame.
              alt: Five frames of a hand picking up a red bowl and placing it on a grey plate, seen from above.
            - video: media/portfolio/phone2panda-act.mp4
              poster: media/portfolio/phone2panda-act-poster.png
              caption: 'Left: a robot demo generated from my recording. Right: the learned ACT policy in a scene it never trained in.'
              alt: A simulated Franka Panda picks up a bowl and places it on a plate, as a generated demo and as the learned policy.
          links:
            - label: Case study
              url: projects/phone2panda/
            - label: Code
              url: https://github.com/LukasWill/phone2panda

        - size: feature
          media: right
          kicker: Real robot · NICOL humanoid
          title: NICOL picks up a can by imitating a human demonstration
          summary: >-
            A run on the physical NICOL humanoid. The arm reaches, grasps, lifts, and
            sets down the can, reproducing a pick that a person demonstrated.
          image: media/portfolio/nicol-picking-poster.jpg
          image_alt: The NICOL humanoid robot grasping and lifting a can from a table.
          video: media/portfolio/nicol-picking-4x.mp4
          credit: Real robot, played at 4× speed.

        - size: feature
          media: top
          title: 'TraceRigor: do RL-trained agents reason better, or only win more?'
          summary: >-
            Does RL training make LLM/VLM agents reason better, or only win more? I built
            the training stack and an automatic reasoning checker to find out, across five
            Qwen2.5 agents.
          points:
            - '**Training.** Multi-turn PPO/GRPO on veRL and Ray, with 128 environments running in parallel at each training step.'
            - '**Checking.** Fast rule checks first, then an LLM judge served with vLLM. Its verdicts match human labels at least 79% of the time.'
            - '**Finding.** RL lifts ALFWorld success from 8.6% to 85.2%, but the runs that win reason barely better than the runs that lose.'
          image: media/portfolio/tracerigor-training.png
          image_alt: Per-checkpoint task performance and reasoning-reliability scores across training for five agents.
          links:
            - label: Project
              url: projects/reasoning-reliability-rl-finetuning/
            - label: Paper
              url: publications/rlvr-agents-reasoning/
            - label: Code
              url: https://github.com/LukasWill/tracerigor

        - size: compact
          summary: Directional VLM rewards pay a robot for visible progress toward the goal, not only for where it is, so it learns manipulation with less training.
          metric:
            value: 78.2%
            label: running-average success on six Meta-World tasks
            compare: vs 63.8% for the best-tuned positional baseline, same training budget
          links:
            - label: Paper
              url: publications/directional-vlm-rewards/
            - label: Code
              url: https://github.com/LukasWill/directional_vlm_rl

        - size: compact
          summary: An LLM agent coordinates both arms of the NICOL humanoid through long-horizon tasks such as pouring, in simulation.
          image: media/portfolio/nicol-bimanual.png
          image_alt: NICOL humanoid grasping two cups, pouring from one into the other, and serving.
          credit: Figure from Chu et al., Humanoids 2024.
          links:
            - label: Paper
              url: publications/llms-orchestrating-bimanual-robots/

        - size: compact
          summary: LLM/VLM planners on the NICOL robot that account for object states such as fresh, bitten, or solid, with a multimodal tabletop benchmark.
          image: media/portfolio/nicol-object-state.png
          image_alt: NICOL robot head beside an apple annotated with object states.
          credit: Figure from Sun et al., ICANN 2024.
          links:
            - label: Paper
              url: publications/object-state-sensitive-task-planning/

        - size: compact
          summary: Q-maps split by reward goal show which goal drives a robot's choice, and a language model can answer questions about them.
          image: media/portfolio/xqmap.png
          image_alt: Composite, colour, and shape Q-maps feeding templated and interactive language explanations.
          credit: Figure from Lu et al., ICDL 2023.
          links:
            - label: Paper
              url: publications/reward-decomposition-robotic-explanations/

  - block: portfolio-expertise
    id: expertise
    content:
      title: Research Focus
      archive_url: projects/
      archive_text: View all projects

  - block: portfolio-publications
    id: publications
    content:
      title: Selected Publications
      text: Peer-reviewed work on RL post-training, robot learning, and agent interpretability.
      archive_url: publications/
      archive_text: View all publications

  - block: portfolio-toolbox
    id: toolbox
    content:
      eyebrow: Toolbox
      title: What I build with
      groups:
        - title: RL post-training
          items: [PPO, GRPO, turn-level GAE, reward models (RLAIF), process rewards]
          evidence:
            - label: TraceRigor
              url: projects/reasoning-reliability-rl-finetuning/
            - label: Curriculum-RLAIF
              url: publications/curriculum-rlaif/
        - title: Training and serving
          items: [PyTorch, veRL (FSDP), Ray, vLLM, Hugging Face Hub]
          evidence:
            - label: TraceRigor
              url: projects/reasoning-reliability-rl-finetuning/
        - title: Robot learning and simulation
          items: [LeRobot, ACT, LIBERO, MuJoCo, Meta-World, ManiSkill]
          evidence:
            - label: phone2panda
              url: projects/phone2panda/
            - label: VLM rewards
              url: publications/directional-vlm-rewards/
        - title: Perception and evaluation
          items: [iPhone LiDAR + ARKit, MediaPipe, ArUco pose estimation, LLM-as-judge]
          evidence:
            - label: phone2panda
              url: projects/phone2panda/
            - label: TraceRigor
              url: projects/reasoning-reliability-rl-finetuning/

  # Temporarily hidden. Uncomment this block to restore homepage updates.
  # - block: portfolio-updates
  #   id: updates
  #   content:
  #     title: Selected Updates
  #     text: Recent research and publication milestones.
  #     count: 3

  - block: portfolio-contact
    id: contact
    content:
      service_title: Professional Service
      service_text: >-
        Conference reviewer for AAMAS, AISTATS, and ICLR 2027; ICLR 2026; AAMAS, AISTATS,
        ICML, ICLR, and NeurIPS 2025; and AISTATS and NeurIPS 2024.
      contact_title: Contact
      contact_text: >-
        I'm looking for research-engineer roles in RL post-training, VLAs and world
        models, and embodied AI. Email is the fastest way to reach me.
      links:
        - text: Email
          url: mailto:wenhao.lu@uni-hamburg.de
        - text: GitHub
          url: https://github.com/LukasWill
        - text: Google Scholar
          url: 'https://scholar.google.com/citations?user=YZt2J_YAAAAJ&hl=de&oi=ao'
        - text: Institutional profile
          url: https://www.inf.uni-hamburg.de/en/inst/ab/wtm/people/lu.html
---
