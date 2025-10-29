---
layout: page
title: Haptic Teleoperation in XR
description: A teleoperation framework for EV battery cell handling, integrating haptic feedback, extended reality (XR) visualization, and adaptive trajectory generation.
img: assets/img/haptic-teleop_project/system_overview.jpg
importance: 2
category: Research
---

This work presents a comprehensive teleoperation framework designed for electric vehicle (EV) battery cell handling. The system combines haptic feedback, extended reality (XR) visualization, and task-parameterized Gaussian mixture regression (TP-GMR) to achieve adaptive, real-time trajectory generation during manipulation tasks.
A key feature of the framework is its variable autonomy mechanism, which allows smooth switching between manual and autonomous operation, giving operators flexible control over the robot’s behavior. To ensure safety during operation, constraint barrier functions (CBFs) are employed to maintain spatial and collision constraints.
Additionally, a lightweight intent prediction module is integrated to anticipate user deviations and precompute corrective trajectories—reducing system response time from approximately 2.0 seconds to under 1 millisecond.
The framework has been implemented on an industrial KUKA robotic manipulator and evaluated in both structured laboratory environments and real-world EV battery disassembly scenarios, demonstrating robust performance, safety, and adaptability in human-in-the-loop robotic applications.

{% include figure.html path="assets/img/haptic-teleop_project/system_overview.jpg" class="img-fluid" title="Methodology" caption="Framework overview" %}

##### Publication

The research conducted in this work has been published in _Journal of Field Robotics_. You can access the full article through the following link:

[Haptic Teleoperation in Extended Reality for Electric Vehicle Battery Disassembly Using Gaussian Mixture Regression](https://doi.org/10.1002/rob.70079)

---
### Experimental Validation

The proposed teleoperation framework was validated using an EV battery module assembly mock-up based on the Mitsubishi Outlander design. A human–robot team performed battery cell placement tasks using haptic feedback and immersive XR visualization.

{% include figure.html path="assets/img/haptic-teleop_project/exp-validation.jpg" class="img-fluid" title="Methodology" caption="" %}

* Scenario 1: A baseline test where a GMR-generated path guided the operator from point A to B without obstacles. The system recorded accuracy, deviations, and completion time.

* Scenario 2: Introduced a spherical obstacle with Constraint Barrier Functions (CBFs) enforcing safety. Deviations triggered automatic replanning, and operator performance was evaluated under dynamic conditions.

* Scenario 3: Extended Scenario 2 by adding predictive intent estimation, allowing the system to anticipate deviations and precompute corrective paths for near-instant replanning.

Five distinct robot start and goal positions were tested across all scenarios to assess adaptability. The experiments confirmed the framework’s safety, responsiveness, and real-time adaptability in EV battery handling tasks.

---

### Evaluation

Each scenario was evaluated against a standard GMR baseline (without replanning). Key performance metrics included traveled distance, force feedback, and replanning efficiency.The combination of XR and haptic feedback led to significant performance improvements. The predictive replanning feature also improved the continuity of force feedback and reduced unnecessary user motion. These results demonstrate a scalable human-in-the-loop solution for semi-structured tasks where full automation is not feasible.

<div class="figure-row">
{% include figure.html path="assets/img/haptic-teleop_project/distance-result.jpg" class="img-fluid" title="Results 1" caption="" %}
{% include figure.html path="assets/img/haptic-teleop_project/force-result.jpg" class="img-fluid" title="Results 2" caption="" %}
</div>

---

### Video Demonstration

Please watch the video for the full demonstration :point_down:

<p align="center">
<iframe
    width="640"
    height="480"
    src="https://www.youtube.com/embed/_colf55RFPw?si=lIMfQZ0Gm-BhxCSy"
    frameborder="0"
    allow="autoplay; encrypted-media"
    allowfullscreen
>
</iframe>
</p>
