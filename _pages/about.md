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

I am currently a Research Engineer at [MMLab@NTU](https://www.mmlab-ntu.com/), Nanyang Technological University, working with [Prof. Chen Change Loy](https://www.mmlab-ntu.com/person/ccloy/). Before that, I completed my MPhil in Advanced Computer Science at the University of Cambridge, where I worked with [Prof. Pietro Liò](https://www.cl.cam.ac.uk/~pl219/) on functional 3D scene-graph grounding, and completed my dissertation with [Prof. Amanda Prorok](https://www.proroklab.org/people/amanda-prorok/) on generalist multi-agent reinforcement learning. Before Cambridge, I spent my final undergraduate year as a research assistant in [Prof. Renjing Xu](https://facultyprofiles.hkust-gz.edu.cn/faculty-personal-page?id=97)'s group at HKUST (Guangzhou), which opened the door to humanoid robotics for me and turned my long-standing fascination with embodied intelligence into a concrete research direction.

I received my BEng in Robotics Engineering from Northwestern Polytechnical University (NWPU), ranking **1st out of 345** students. During my undergraduate years, I was deeply involved in robotics competitions and real-world robot development, including RoboCup China, and served as captain of the rescue-robotics team at our robotics base. These experiences shaped my belief that impactful robotics research should not only produce elegant models, but also systems that work when the world becomes messy.

My CV is available [**here**](/images/Mingqian_Zhou_CV.pdf).

# 🔥 News
- *2026.10*: &nbsp; Joined **MMLab@NTU** as a Research Engineer, working with Prof. Chen Change Loy.
- *2026.10*: &nbsp;🎉 Kimodo-Policy preprint released ([project page](https://kimodo-policy.github.io/script/)).
- *2026.09*: &nbsp; LumiBench, a benchmark for illumination robustness in robotic manipulation, submitted and under review.
- *2026.05*: &nbsp; GEAR, my first-author work on functional 3D scene-graph grounding, is in preparation (target: IEEE RA-L).
- *2026.03*: &nbsp;🎉 Dream2Act preprint released on **arXiv** ([arXiv:2603.19709](https://arxiv.org/abs/2603.19709)).
- *2025.09*: &nbsp; Completed real-world zero-shot humanoid deployment on a full-sized Unitree G1.
- *2025.09*: &nbsp;🎓 Graduated from NWPU as an **Outstanding Graduate** and started my MPhil at Cambridge.

# 📝 Papers & Preprints
{: #publications}

<div class='paper-box'><div class='paper-box-image'><div><div class="badge">arXiv 2026</div><img src='images/kimodo.png' alt="Kimodo-Policy" width="100%"></div></div>
<div class='paper-box-text' markdown="1">

**Kimodo-Policy: From Text-to-Motion Generators to Humanoid Vision-Language-Action Policies**

Yunheng Wang\*, Jiaxi Zhang\*, Wei Lu\*, Yuetong Fang, Taowen Wang, Yixiao Feng, Shuning Zhang, Junzhe Xu, Yichi Wang, Zizhao Yuan, Kailun Huang, Lusong Li, **<u>Mingqian Zhou</u>**, Zecui Zeng, Renjing Xu &nbsp;<span style="font-size:.88em;color:#777;">(\*equal contribution; Zecui Zeng and Renjing Xu, corresponding authors)</span>

*arXiv preprint 2026*

<a href="https://kimodo-policy.github.io/script/" style="display:inline-block;padding:1px 11px;margin:3px 6px 3px 0;border:1px solid #00369f;border-radius:6px;color:#00369f;font-size:.84em;font-weight:600;text-decoration:none;">🌐 Project Page</a><a href="https://github.com/kimodo-policy/kimodo-policy.github.io/releases/download/web-v1/main_arxiv.copy.pdf" style="display:inline-block;padding:1px 11px;margin:3px 6px 3px 0;border:1px solid #00369f;border-radius:6px;color:#00369f;font-size:.84em;font-weight:600;text-decoration:none;">📑 PDF</a>

- Kimodo-Policy builds a humanoid vision-language-action policy on top of a pretrained text-to-motion model, so the policy starts from whole-body motion priors instead of learning coordination from scratch. Actions are generated in three stages (root → body → hand). With 678M parameters (92M trainable), it reaches **72.14%** overall success on HumanoidArena, best or joint-best results on six of eight SIMPLE tasks, and **60%** mean success on real-world loco-manipulation tasks.
</div>
</div>

<div class='paper-box'><div class='paper-box-image'><div><div class="badge">Under Review</div><img src='images/lumibench.png' alt="LumiBench" width="100%"></div></div>
<div class='paper-box-text' markdown="1">

**LumiBench: Benchmarking Illumination Robustness in Robotic Manipulation Policies**

… **<u>Mingqian Zhou</u>** … &nbsp;<span style="font-size:.88em;color:#777;">(full author list withheld during anonymous review)</span>

*Under review, 2026*

<a href="https://victor-roboneo.github.io/LumiBench/" style="display:inline-block;padding:1px 11px;margin:3px 6px 3px 0;border:1px solid #00369f;border-radius:6px;color:#00369f;font-size:.84em;font-weight:600;text-decoration:none;">🌐 Project Page</a>

- LumiBench sorts lighting changes by physical mechanism (intensity, color, uneven lighting, flicker, moving shadows) and tests each one against the same rollout under normal light. Built on RoboTwin 2.0 with five policy families and ten tasks, plus real-robot checks. Robustness depends heavily on the policy, task, and lighting type: OpenVLA-OFT keeps **88.3%** of its normal-light success under perturbation, while FastWAM keeps **46.1%** despite scoring higher under normal light.
</div>
</div>

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

<div class='paper-box'><div class='paper-box-image'><div><div class="badge">Cambridge · 2025–26</div><img src='images/marl.png' alt="Multi-Agent RL" width="100%"></div></div>
<div class='paper-box-text' markdown="1">

**Learning Cooperative Primitives for Multi-Task Multi-Agent Reinforcement Learning**

MPhil Dissertation, *Prof. Amanda Prorok*, University of Cambridge · 2025–2026

- Developed a foundation-model-inspired generalist policy that learns reusable cooperative primitives for zero-shot transfer across unseen multi-agent tasks, using graph-based attentional communication, VMAS curricula, and BenchMARL evaluation against MARL baselines such as MAPPO.
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

**Scholarships**
- *2024* &nbsp; **National Scholarship Nominee**
- *2023* &nbsp; **"Suzhou Yucai" Special Scholarship**
- *2022, 2023, 2024* &nbsp; **First-Class Scholarship**
- *2022* &nbsp; **"Kewei" Special Scholarship**

**Honors**
- *2025* &nbsp; **Outstanding Graduate of NWPU**
- *2023* &nbsp; **Star of Erudition**
- *2022, 2023, 2024* &nbsp; **Merit Student, NWPU**

**Competitions**
- *2023.08* &nbsp; **Outstanding Winner**, Elite League of the National 3D Competition
- *2023.04* &nbsp; **Meritorious Winner**, Mathematical Contest in Modeling (MCM/ICM)
- *2022.11* &nbsp; **National First Prize**, Rescue Robot (Obstacle &amp; Search-and-Rescue), 2022 China Robot Competition (RoboCup China)
- *2022.11* &nbsp; **National Second Prize**, Rescue Robot (Autonomous Mapping), 2022 China Robot Competition (RoboCup China)

# 💼 Experience

<style>
.inst{display:flex;align-items:center;gap:40px;padding:22px 0;border-bottom:1px solid #eee;}
.inst-logo{flex:0 0 120px;display:flex;justify-content:center;}
.inst-logo img{max-width:120px;max-height:120px;width:auto;height:auto;}
.inst-name{font-size:1.12em;font-weight:600;margin-bottom:6px;}
.inst-line{margin-top:3px;}
@media (max-width:600px){.inst{gap:18px;}.inst-logo{flex-basis:72px;}.inst-logo img{max-width:72px;max-height:72px;}}
</style>
<div class="inst">
<div class="inst-logo"><img src="images/logos/ntu.png" alt="NTU logo"></div>
<div class="inst-text">
<div class="inst-name"><a href="https://www.ntu.edu.sg/">Nanyang Technological University</a></div>
<div class="inst-line"><b>2026.10 – Present</b> · <i>Research Engineer</i></div>
<div class="inst-line"><a href="https://www.mmlab-ntu.com/">MMLab@NTU</a></div><div class="inst-line">Supervisor: <a href="https://www.mmlab-ntu.com/person/ccloy/">Prof. Chen Change Loy</a></div>
</div>
</div>
<div class="inst">
<div class="inst-logo"><img src="images/logos/hkust-gz.png" alt="HKUST(GZ) logo"></div>
<div class="inst-text">
<div class="inst-name"><a href="https://www.hkust-gz.edu.cn/">The Hong Kong University of Science and Technology (Guangzhou)</a></div>
<div class="inst-line"><b>2025.01 – 2025.09</b> · <i>Research Assistant</i></div>
<div class="inst-line">Humanoid whole-body control</div><div class="inst-line">Advisor: <a href="https://facultyprofiles.hkust-gz.edu.cn/faculty-personal-page?id=97">Prof. Renjing Xu</a></div>
</div>
</div>

# 📖 Education

<div class="inst">
<div class="inst-logo"><img src="images/logos/cambridge.png" alt="University of Cambridge logo"></div>
<div class="inst-text">
<div class="inst-name"><a href="https://www.cam.ac.uk/">University of Cambridge</a></div>
<div class="inst-line"><b>2025.09 – 2026.06</b> · <i>MPhil in Advanced Computer Science</i></div>
<div class="inst-line"><a href="https://www.cst.cam.ac.uk/">Department of Computer Science and Technology</a></div><div class="inst-line">Supervisors: <a href="https://www.cl.cam.ac.uk/~pl219/">Prof. Pietro Liò</a> and <a href="https://www.proroklab.org/people/amanda-prorok/">Prof. Amanda Prorok</a></div>
</div>
</div>
<div class="inst">
<div class="inst-logo"><img src="images/logos/nwpu.png" alt="NWPU logo"></div>
<div class="inst-text">
<div class="inst-name"><a href="https://en.nwpu.edu.cn/">Northwestern Polytechnical University</a></div>
<div class="inst-line"><b>2021.09 – 2025.06</b> · <i>BEng in Robotics</i></div>
<div class="inst-line">91.36/100 · rank 1/345 · Outstanding Graduate</div>
</div>
</div>
<div class="inst">
<div class="inst-logo"><img src="images/logos/khalifa.png" alt="Khalifa University logo"></div>
<div class="inst-text">
<div class="inst-name"><a href="https://www.ku.ac.ae/">Khalifa University</a></div>
<div class="inst-line"><b>2023.08 – 2023.12</b> · <i>Exchange Student</i></div>
<div class="inst-line">Electrical Engineering · GPA 4.0/4.0</div>
</div>
</div>
