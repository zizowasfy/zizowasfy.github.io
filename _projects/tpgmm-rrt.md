---
layout: page
title: Task-Parameterized Motion Planner
description: Efficient motion planning for robotic manipulation in constrained environments using GMM-Informed RRT planners.
img: assets/img/tpgmm-rrt_project/tpgmm-rrt-preview.jpg
importance: 3
category: Research
---

This project introduces novel GMM-Informed RRT planners (GMM-RRT and GMR-RRT) designed to enhance motion planning efficiency and path optimality for robotic manipulation in constrained environments. By integrating Task-Parameterized Gaussian Mixture Models (TP-GMM), trained on human demonstrations, with sampling-based RRT planners, the system generates task-adaptive sampling distributions that guide the search towards feasible and high-quality solutions.

The approach involves projecting tasks to joint space using Jacobian-based inverse kinematics. Implemented within the MoveIt framework, the planners were rigorously evaluated through simulations and 30 real-world Electric Vehicle (EV) battery disassembly trials. Results demonstrate superior performance over baseline planners, yielding significantly shorter paths, reducing path simplification time, and maintaining a 100% success rate.

##### Publication

The research conducted in this project has been published in _Robotics and Computer-Integrated Manufacturing_ Journal. You can access the full article through the following link:

[Task-Parameterized GMM-Informed RRT Planners for Robotic Manipulation in Constrained Environments](https://doi.org/10.1016/j.rcim.2025.103095)

<div class="text-center">
  {% include figure.html path="assets/img/tpgmm-rrt_project/system_overview.jpg" class="img-fluid" caption="System Overview" %}
</div>

---

### Experimental Setup

The experimental environment featured a 7-DOF Panda robotic arm operating in a workspace designed to simulate EV battery disassembly. The setup included scattered obstacles representing battery pack components, target objects such as bolts, and a placeholder area for disassembled parts.
Depth data from the RealSense camera were processed into a point cloud, then converted into an octomap—a 3D occupancy grid that offers a probabilistic and compact representation of the environment. Within the MoveIt framework, the octomap enhanced motion planning, collision detection, and path optimization, enabling safer navigation in cluttered environments.
To ensure a reliable simulation-to-reality (sim-to-real) transition, the depth camera was fixed and precisely calibrated with respect to the robot base. The same transformations were mirrored in simulation, allowing real-world depth data to be projected directly into the simulated planning scene.

{% include figure.html path="assets/img/tpgmm-rrt_project/tpgmm-rrt-preview.jpg" class="img-fluid" title="Experimental Setup" caption="Experimental setup" %}

### Visual  Results

The experimental design included five distinct setups per planner, each repeated across ten independent trials, resulting in 50 trials per planner. These setups introduced variability through different obstacle configurations and start/goal poses, ensuring a diverse set of motion planning challenges.
All start, goal, and obstacle positions were uniformly sampled within a bounded workspace relative to the robot’s base, providing a consistent and unbiased evaluation of planner performance across all scenarios.
The following images show the results from the benchmark experiments, demonstrating the path efficiency of the developed GMM-Informed planners.

<div class="figure-row">
{% include figure.html path="assets/img/tpgmm-rrt_project/simulation-exps.jpg" class="img-fluid" caption="Simulation experiments" %}
{% include figure.html path="assets/img/tpgmm-rrt_project/real-exps.jpg" class="img-fluid" caption="Real-world experiments" %}
</div>

---

### Video Demonstration

Please watch the video for the full demonstration :point_down:

<p align="center">
<iframe
    width="640"
    height="480"
    src="https://www.youtube.com/embed/LZvEhICvIQ0"
    frameborder="0"
    allow="autoplay; encrypted-media"
    allowfullscreen
>
</iframe>
</p>
