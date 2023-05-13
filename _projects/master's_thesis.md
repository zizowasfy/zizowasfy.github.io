---
layout: page
title: Master's Thesis
description: Comparative analysis of a Peg-In-Hole
img: assets/img/bachelor's_thesis.jpg
importance: 2
category: Master's
---

This is the very first project I got introduced to working with ROS, intensely. My team and I were the first to work on such application in the region. We participated with the project in a couple of regional competitions: 

> 
* DELL EMC Technologies annual challenge for graduation projects from senior undergraduate students 2022. (Awarded the 5th place :dart:)
* Egypt IOT & AI challenge competition, graduation projects category 2020. (Awarded the 1st place :trophy:)

My Bachelor’s Thesis had two scopes, controlling a Teleoperated custom-made 7 DOF serial arm manipulator hardware from a VR scene, and modeling the robot with a Neural Network architecture to solve the Inverse Kinematics. First, using ROS, the robot's URDF model is imported in ROS visualization environment and using ROS’s tools to visulaize motion planning and execution to defined points in the robot’s workspace. Furthermore, Unity3D game engine was used as the platform for integrating VR kit (headset and controllers). After creating a scene in Unity, a ROS-Unity teleoperated connection is established through a local network with the use of ROS-Sharp libraries and tools. Hence, when the user puts on the VR kit, enters the scene, and moves the robot in the Unity scene, the motion of the robot is transferred to the robot’s actual hardware body, thus moving to the desired position given by the user from the VR Unity scene. 

On the other hand, we designed our own deep neural network (DNN) for training the robot to cover its workspace and create its own model without the use of conventional Inverse kinematics method. 
I was mainly responsible for developing the hardware, parsing the URDF into ROS and Unity, motion planning and execution of the robot, and establishing the connection between ROS and all other platforms (nodes) used, Unity3D, Gazebo simulation tool, Keras-Python, and hardware’s microcontroller.

Please refer to the Video for more details :point_down:

<p align="center">
<iframe
    width="640"
    height="480"
    src="https://www.youtube.com/embed/oxwMDySRGDk"
    frameborder="0"
    allow="autoplay; encrypted-media"
    allowfullscreen
>
</iframe>
</p>

