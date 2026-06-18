---
permalink: /
title: ""
excerpt: ""
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

<span class='anchor' id='about-me'></span>

Hi, I'm **Mingqian Zhou (周鸣谦)**. My research is driven by a simple question: how can algorithms leave the screen and make intelligent, reliable decisions in the physical world? I am particularly interested in enabling humanoid robots to perform useful tasks in unstructured real-world environments, which brings my work to the intersection of humanoid whole-body control, sim-to-real reinforcement learning, and action-grounded 3D scene understanding.

I am currently an MPhil student in Advanced Computer Science at the University of Cambridge, where I work with [Prof. Pietro Liò](https://www.cl.cam.ac.uk/~pl219/) on functional 3D scene-graph grounding, and completed my dissertation with [Prof. Amanda Prorok](https://www.proroklab.org/) on generalist multi-agent reinforcement learning. Before Cambridge, I spent my final undergraduate year as a research assistant at HKUST (Guangzhou) with [Prof. Renjing Xu](https://facultyprofiles.hkust-gz.edu.cn/faculty-personal-page?id=97), where I led the real-world deployment of **Dream2Act** on a full-sized Unitree G1 humanoid robot. That experience turned my long-standing fascination with embodied intelligence into a concrete research direction.

I received my BEng in Robotics Engineering from Northwestern Polytechnical University (NWPU), ranking **1st out of 345** students. During my undergraduate years, I was deeply involved in robotics competitions and real-world robot development, including RoboCup China, and served as captain of the rescue-robotics team at our robotics base. These experiences shaped my belief that impactful robotics research should not only produce elegant models, but also systems that work when the world becomes messy.

My CV is available [**here**](/images/Mingqian_Zhou_CV.pdf).

<div style="background:#f5f8fc;border:1px solid #e3e9f2;border-left:4px solid #00369f;border-radius:10px;padding:16px 20px;margin:20px 0;">
<div style="font-weight:700;font-size:1.08em;margin-bottom:8px;">🎯 Looking For</div>
<div style="margin-bottom:8px;"><b>Research / RA / visiting positions</b> from <b>August 2026</b> (6–9 months) &nbsp;·&nbsp; <b>PhD positions</b> starting <b>Fall 2027</b></div>
<div style="margin-bottom:4px;">in embodied AI and robot learning, especially:</div>
<ul style="margin:0 0 10px;padding-left:1.25em;">
<li>Humanoid learning &amp; whole-body control</li>
<li>Sim-to-real reinforcement learning</li>
<li>World models for embodied agents</li>
<li>Vision-language-action models</li>
</ul>
<div>📩 <a href="mailto:mz560@cam.ac.uk">mz560@cam.ac.uk</a></div>
</div>

# 🔥 News
- *2026.05*: &nbsp; GEAR, my first-author work on functional 3D scene-graph grounding, is in preparation (target: IEEE RA-L).
- *2026.03*: &nbsp;🎉 Dream2Act preprint released on **arXiv** ([arXiv:2603.19709](https://arxiv.org/abs/2603.19709)).
- *2025.09*: &nbsp; Completed real-world zero-shot humanoid deployment on a full-sized Unitree G1.
- *2025.09*: &nbsp;🎓 Graduated from NWPU as an **Outstanding Graduate** (top 1%) and started my MPhil at Cambridge.

# 📝 Papers & Preprints
{: #publications}

<div class='paper-box'><div class='paper-box-image'><div><div class="badge">In Prep</div><img src='images/gear.png' alt="GEAR" width="100%"></div></div>
<div class='paper-box-text' markdown="1">

**GEAR: Gated Evidence-Aware Routing for Functional 3D Scene Graph Grounding**

**<u>Mingqian Zhou</u>**, Dennis Rotondi, Andrea Giuseppe Di Francesco, Renjing Xu, Pietro Liò

*Manuscript in preparation — target: IEEE RA-L*

- GEAR studies *when* expensive LLM-based graph verification is actually worth calling for functional 3D scene-graph grounding. It pairs a structured graph prior with a validation-frozen router that invokes the LLM verifier only when it helps — reaching **0.7075** overall R@1 while keeping verifier calls low (**58.1%** verifier invocation, ≈**14.7%** normalized API cost). I also built **FunGraph-Bench**, a 1,412-query benchmark over SceneFun3D and 3DSSG with target, anchor, supporting-edge, and same-label-distractor annotations.
</div>
</div>

<div class='paper-box'><div class='paper-box-image'><div><div class="badge">arXiv 2026</div><img src='images/dream2act.png' alt="Dream2Act" width="100%"></div></div>
<div class='paper-box-text' markdown="1">

**Dream2Act: Morphology-Consistent Humanoid Interaction through Robot-Centric Video Synthesis**

Weisheng Xu\*, Jian Li\*, Yi Gu, Bin Yang, Haodong Chen, Shuyi Lin, **<u>Mingqian Zhou</u>**, et al. &nbsp;<span style="font-size:.88em;color:#777;">(\*equal contribution; Renjing Xu, corresponding author)</span>

*arXiv 2026 (arXiv:2603.19709)*

<a href="https://wesleyxu224.github.io/Dream2Act/" style="display:inline-block;padding:1px 11px;margin:3px 6px 3px 0;border:1px solid #00369f;border-radius:6px;color:#00369f;font-size:.84em;font-weight:600;text-decoration:none;">🌐 Project Page</a><a href="https://arxiv.org/abs/2603.19709" style="display:inline-block;padding:1px 11px;margin:3px 6px 3px 0;border:1px solid #00369f;border-radius:6px;color:#00369f;font-size:.84em;font-weight:600;text-decoration:none;">📄 arXiv</a><a href="https://wesleyxu224.github.io/Dream2Act/static/pdfs/dream2act.pdf" style="display:inline-block;padding:1px 11px;margin:3px 6px 3px 0;border:1px solid #00369f;border-radius:6px;color:#00369f;font-size:.84em;font-weight:600;text-decoration:none;">📑 PDF</a><a href="https://github.com/WesleyXu224/Dream2Act_Code" style="display:inline-block;padding:1px 11px;margin:3px 6px 3px 0;border:1px solid #00369f;border-radius:6px;color:#00369f;font-size:.84em;font-weight:600;text-decoration:none;">💻 Code</a>

- Dream2Act uses video generation models as zero-shot physical simulators, hallucinating interaction video in the robot's own morphology from a single third-person image — sidestepping the morphology gap of human-to-robot retargeting. Evaluated on the Unitree G1 across four whole-body interaction tasks, it reaches **37.5%** overall task success vs **0%** for retargeting baselines.
- **My contribution:** I led the real-world deployment on the Unitree G1 — building the on-robot execution pipeline (global-trajectory solver + constrained IK) and running the hardware experiments.
</div>
</div>

# 🔬 Research Experience

<div class='paper-box'><div class='paper-box-image'><div><div class="badge">HKUST(GZ) · 2025</div><img src='images/humanoid_wbc.png' alt="Humanoid WBC" width="100%"></div></div>
<div class='paper-box-text' markdown="1">

**Learning Human-to-Humanoid Real-Time Whole-Body Control**

Research Assistant, *Prof. Renjing Xu*, HKUST (Guangzhou) · Jan.–Sep. 2025

- Built a learning-based whole-body control framework for real-time human-to-humanoid motion imitation, with a scalable sim-to-data pipeline (privileged motion imitator + large-scale retargeting) and an RL policy reaching zero-shot Sim-to-Real transfer on a Unitree G1 (e.g., boxing, kicking).
</div>
</div>

<div class='paper-box'><div class='paper-box-image'><div><div class="badge">Cambridge · Ongoing</div><img src='images/marl.png' alt="Multi-Agent RL" width="100%"></div></div>
<div class='paper-box-text' markdown="1">

**Learning Cooperative Primitives for Multi-Task Multi-Agent Reinforcement Learning**

Graduate Researcher, *Prof. Amanda Prorok*, University of Cambridge · Ongoing

- Developing a foundation-model-inspired generalist policy that learns reusable cooperative primitives for zero-shot transfer across unseen multi-agent tasks, using graph-based attentional communication, VMAS curricula, and BenchMARL evaluation against MARL baselines such as MAPPO.
</div>
</div>

<div class='paper-box'><div class='paper-box-image'><div><div class="badge">NWPU · 2023–24</div><img src='images/bipedal.png' alt="Bipedal Robots" width="100%"></div></div>
<div class='paper-box-text' markdown="1">

**Dynamic Reactive Motion Planning of Bipedal Robots**

Research Assistant, *Prof. Zhaohui Yuan*, NWPU · Apr. 2023 – Jun. 2024

- Developed a hierarchical MPC/WBC framework for stable bipedal locomotion under external disturbances, proposing a Linear Reaction Wheel Pendulum MPC for online gait generation, validated in whole-body simulation and NAO hardware experiments.
</div>
</div>

<div class='paper-box'><div class='paper-box-image'><div><div class="badge">NWPU · 2022–23</div><img src='images/rescue.png' alt="Rescue Robot" width="100%"></div></div>
<div class='paper-box-text' markdown="1">

**Robust Perception and Navigation for Rescue Robots**

Project Leader, *Prof. Wentao Jiang*, NWPU · Jun. 2022 – Dec. 2023

- Led a GPS-denied autonomous navigation system for post-disaster environments combining Cartographer SLAM, A\* global planning, DWA local control, and LiDAR–camera semantic fusion, improving localization accuracy by 30% over a Gmapping baseline.
</div>
</div>

# 🎖 Honors and Awards

**Scholarships &amp; Honors**
- *2025* &nbsp; **Outstanding Graduate of NWPU** (top 1%)
- *2024* &nbsp; **National Scholarship**; **Model Student Pacesetter** — highest honor for undergraduates at NWPU
- *2023* &nbsp; **"Su Zhou Yu Cai" Special Scholarship** (highest scholarship at NWPU); **Star of Erudition** (1/345)
- *2021–2024* &nbsp; **Merit Student of NWPU** (top 5%, four consecutive years)

**Competitions**
- *2023.11* &nbsp; **Provincial Second Prize**, China Undergraduate Mathematical Contest in Modeling (CUMCM)
- *2023.10* &nbsp; **National Third Prize**, 2023 RoboCup China
- *2023.09* &nbsp; **Meritorious Winner**, Mathematical Contest in Modeling (MCM/ICM) — top 6%
- *2023.08* &nbsp; **Outstanding Winner**, Elite League of the National 3D Competition
- *2023.08* &nbsp; **National Third Prize**, China Intelligent Robot Innovation Competition
- *2022.11* &nbsp; **Champion**, 2022 China Robot Competition &amp; RoboCup China
- *2022.07* &nbsp; **International Third Prize**, Asia-Pacific Mathematical Contest in Modeling (APMCM)

# 📖 Education
- *2025.09 – 2026.06*, **University of Cambridge** — MPhil in Advanced Computer Science (expected Distinction)
- *2021.09 – 2025.06*, **Northwestern Polytechnical University** — BEng in Robotics (91.36/100, rank 1/345)
- *2023.08 – 2023.12*, **Khalifa University** (exchange) — Electrical Engineering (GPA 4.0/4.0)
