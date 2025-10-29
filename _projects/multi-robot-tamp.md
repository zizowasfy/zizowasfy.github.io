---
layout: page
title: Multi-Robot Task and Motion Planning
description: A Task and Motion Planning (TAMP) framework for multi-robot EV battery disassembly, combining symbolic task planning, vision-based perception, and learned motion generation.
img: assets/img/multi-robot-tamp_project/dual-arm_env.jpg
importance: 1
category: Research
---

This work introduces a four-layer task-and-motion planning (TAMP) framework to enable precise and efficient multi-robot coordination for electric-vehicle (EV) battery disassembly. The system is designed to handle cluttered and dynamic environments by integrating symbolic task planning with a motion planner guided by demonstrations (TP-GMM).

Real-time component localization is achieved using stereo vision with YOLOv8, while a combination of OctoMap-based 3D mapping and the Flexible Collision Library (FCL) in MoveIt ensures robust collision avoidance. This unifies predictive digital-twin collision checking with reactive, vision-based safety measures.

{% include figure.html path="assets/img/multi-robot-tamp_project/dual-arm_env.jpg" class="img-fluid" title="System Overview" caption="Multi-robot disassembly setup" %}

##### Publication

This research has been submitted for publication. Pending decision!

---

### TAMP Framework and Results

The framework was validated on a system with two UR10e robots performing various disassembly tasks, including cable, busbar, service plug, and leaf-cell removals. The performance of the proposed approach was compared against a default RRTConnect baseline.

The results demonstrated significant improvements in motion efficiency and safety. The average end-effector path length was reduced by 63.3%, and the makespan (total time) decreased by 8.1%. Furthermore, the swept volumes of the robot arms were substantially smaller, and the mutual overlap between the robots' workspaces decreased by 47%.

These findings highlight the framework's ability to produce more compact, safer, and more efficient motions, advancing the autonomy and precision of multi-robot systems for EV battery disassembly in unstructured environments.

---

### Video Demonstration

Please watch the video for the full demonstration :point_down:

<p align="center">
<iframe
    width="640"
    height="480"
    src="https://www.youtube.com/embed/VJEolRomaQM?si=_J0EiWQAb9jWZMdw"
    frameborder="0"
    allow="autoplay; encrypted-media"
    allowfullscreen
>
</iframe>
</p>