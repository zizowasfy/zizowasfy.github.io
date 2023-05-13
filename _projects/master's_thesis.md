---
layout: page
title: Master's Thesis
description: Comparative analysis of a Peg-In-Hole
img: assets/img/master's_thesis.jpg
importance: 1
category: Master's
---

Tight clearances have always been a posing challenge while performing industrial assembly tasks. In many cases, robotic systems have positional errors larger than the clearance between assembly parts of the task. A Peg-In-Hole setup, with clearance 0.3 mm, is utilized in this thesis to conduct experiments of different approaches: Autonomous, Shared, Offline LfD, and Online LfD. We measure the Success Rate (SR) and Completion Time (CT) as performance indicators in all experiments.
AUTO:
The Peg picking part is done autonomously using (Deep Learning and/or Classical) CV techniques to detect the random peg position from the starting area. The Peg insertion part is done using generated masks to detect the hole position; thus, complete the Peg-In-Hole task.
SHARED:
The task is performed autonomously until a termination condition occurs; whether the autonomous searching time reaches a timeout or the user decides to take over the control. The user then completes the task via Bi-lateral Tele-operation system.
Learning from Demonstration (LfD):
User teleoperated demonstrations (or trials) are utilized to learn a Gaussian Mixture Model (GMM) model encoding the task trajectory in 3D space. Gaussian Mixture Regression (GMR) is used to infer a learned trajectory for performing the Peg-In-Hole task. In this work, 2 LfD frameworks are developed and experimented with a number of 20 trials for the Peg-In-Hole:
- Offine LfD -- First, the user record the demonstrations (3 demonstrations),  learned trajectory is generated, and lastly, the 20 trials are performed using that learned trajectory.
- Online LfD -- During any trial of the 20 trials, the user can take over the control (SHARED) and correct or adjust the trajectory which is recorded as a demonstration for the LfD framework. Hence, the learned trajectory is continuously enhanced throughout the 20 trials of the Peg-In-Hole task.

Please refer to the Video for more details :point_down:

<p align="center">
<iframe width="560" height="315" 
src="https://www.youtube.com/embed/2F8oRTPPH9U"
 title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>

</p>

