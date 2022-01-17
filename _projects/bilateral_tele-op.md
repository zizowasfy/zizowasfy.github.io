---
layout: page
title: Internship
description: Bilateral Tele-operation of Kuka Iiwa via Touch haptic device
img: assets/img/internship.jpg
importance: 2
category: Master's
---

This project is considered the starting point for my ongoing Master's thesis.

I spent my summer internship 2021 in the Intelligent lab of robotics at Innopolis University, supervised by Professor Igor Gaponov, who is my masters thesis supervisor, to establish a teleoperation scheme between the Kuka Iiwa robot and Touch haptic device. The Kuka Iiwa is programmed in Java and with using ROSSmartServo application, the Kuka Iiwa is connected to ROS melodic on Ubuntu 18. On the other hand, the Touch haptice device runs on a C++ program on Windows 10. Therefore, ROS Windows is setup on Windows and hence the Touch can connect to ROS. 

By the end of the internship, I have successfully established a bilateral teleoperation system with the Iiwa robot being the 'slave' manipulator and the haptic device being the 'master' manipulator. The system supports telemanipulation in both joint and cartesian spaces while a continuous force-feedback from Iiwa to Touch is maintained. 

Please watch the video for the complete demo :point_down:

<p align="center">
<iframe
    width="640"
    height="480"
    src="https://www.youtube.com/embed/veS7uErQFMY"
    frameborder="0"
    allow="autoplay; encrypted-media"
    allowfullscreen
>
</iframe>
</p>

