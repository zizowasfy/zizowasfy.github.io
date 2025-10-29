---
layout: page
title: Tele-robotics for Disassembly
description: A comparative study of telerobotic systems for the disassembly of electric vehicle batteries, focusing on the impact of haptic feedback on task performance.
img: assets/img/tele-robotics_project/disassembly_process.jpg
importance: 4
category: Research
---

This research investigates the use of telerobotics for the disassembly of electric vehicle (EV) batteries, a critical step for recycling and reusing valuable materials. The work addresses the challenges of battery disassembly, such as design complexity and safety concerns, by exploring semi-autonomous robotic solutions.

A comparative study was conducted between two haptic telerobotic frameworks: a traditional asymmetric master-slave setup and a system with identical master and slave cobots. The disassembly of a Nissan Leaf 2011 module stack was used as a benchmark to evaluate the systems based on task completion time and success rate.

{% include figure.html path="assets/img/tele-robotics_project/system_overview.jpg" class="img-fluid" title="System Overview" caption="Telerobotic disassembly setup" %}

##### Publication

The findings of this study have been published in _Frontiers in Robotics and AI_. The full article can be accessed through the link below:

[Towards Reuse and Recycling of Lithium-ion Batteries: Tele-robotics for Disassembly of Electric Vehicle Batteries](https://doi.org/10.3389/frobt.2023.1179296)

---

### Comparative Study

<div class="figure-row">
{% include figure.html path="assets/img/tele-robotics_project/franka_master.jpg" class="img-fluid" title="Results 1" caption="" %}
{% include figure.html path="assets/img/tele-robotics_project/haptic_master.jpg" class="img-fluid" title="Results 2" caption="" %}
</div>

The study revealed that using identical cobots for master and slave devices resulted in a significant time reduction of 22%–57% for various disassembly tasks. This improvement was primarily attributed to the expanded workspace and 1:1 positional mapping.

{% include figure.html path="assets/img/tele-robotics_project/time_result.jpg" class="img-fluid" title="System Overview" caption="" %}

However, this configuration also led to a 10%–30% decrease in the first-attempt success rate. The research found that for tasks like unbolting and grasping, the realism of force feedback was less critical than the directional information. In contrast, for vacuum pick-and-place and contact cutting tasks, 1:1 force mapping provided stronger tactile cues from the environment, improving performance.

These results highlight the trade-offs between different telerobotic setups and provide valuable insights for designing effective systems for complex manipulation tasks in hazardous environments.

---

### Experiments Demonstration

Please watch the video of the experiments recorded for different disassembly processes :point_down:

<p align="center">
<iframe
    width="640"
    height="480"
    src="https://www.youtube.com/embed/8cJ5QBYGtnU?si=M3fTcXG6q0w2iDjn"
    frameborder="0"
    allow="autoplay; encrypted-media"
    allowfullscreen
>
</iframe>
</p>