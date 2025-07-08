---
layout: post
title: Try DeepMimic in Isaacgym with our assignment
date: 2025-07-08 17:06:13
description: A public repo for imitating human motions in a physics-simulator using RL
tags: RL, Animation, Robotics
categories: Code
tabs: true
---

This spring semester, I was a teaching assistant for the course [Computational Models of Motion](https://crl.ethz.ch/teaching/computational-motion-25/), which is a MSc. level course offered at ETH.
This course lies between robotics and animation and includes topics such as inverse kinematics (IK), trajectory optimization, RL, as well as up-to-date research topics such as motion manifolds and generative motion synthesis. 

For this course, I developed a coding assignment for implementing the DeepMimic[1] paper using Isaacgym. The goal was to give students hands-on experience with using RL to imitate complex character motions (Cartwheeling!) in a high-performance physics simulator.

<div class="row mt-3">

    <div class="col-sm mt-3 mt-md-0">

        {% include figure.liquid loading="eager" path="assets/img/post_images/cartwheel_mimic.gif" class="img-fluid rounded z-depth-1" %}

    </div>

</div>


Many of the students managed to complete this assignment, which makes me excited! And I'm here to say that the code is publicly available, so if you want to get your hands dirty with RL and motion imitation, you can start here: [Github](https://github.com/CMM-25/a3)

Although we used AWS for the course, you can run the docker on any system that has a sufficiently powerful Nvidia gpu for running Isaacgym.

Feedback, ideas, and contributions are always welcome. I hope it helps others get started with RL-based character control and sparks some fun experiments!

# References
[1] Peng, Xue Bin, et al. "Deepmimic: Example-guided deep reinforcement learning of physics-based character skills." ACM Transactions On Graphics (TOG) 37.4 (2018): 1-14.