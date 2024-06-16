---
layout: post
title: "Softwares Overview"
date: 2024-06-01
categories: Softwares
excerpt: "A brief summary of the softwares focusing on key discussions and findings..."
---

## Franka KIT

<img src="../assets/franka/franka_kit.svg" alt="Franka KIT Overview" style="width: 400px; height: auto;">

### Franka KIT Features

**Support for Various Sensors**
- Includes integration with internal robot sensors and depth cameras, enhancing the robot's perception and interaction capabilities.

**Pre-designed Tasks**
- Comes with pre-designed tasks such as reach and push, allowing for quick deployment and testing of robotic functions.

**Parallel Training**
- Supports parallel training on multiple robots within the Gazebo simulation environment, facilitating scalable and efficient robot learning.

**Visualization Capabilities**
- Offers advanced visualization tools to monitor robot operations and training processes in real-time.

**Integration with Robotics Toolbox**
- Fully integrated with the robotics toolbox, providing essential tools for inverse and forward kinematics, as well as dynamic calculations.

**Autonomous Learning Library**
- Utilizes a comprehensive autonomous learning library designed for developing, testing, and evaluating new algorithms directly on the robot.


### Demonstrations from Datasets
In the first part of our demonstrations, we used an episode from the [Viola](https://www.tensorflow.org/datasets/catalog/viola) dataset and ran it on the real robot. The visual comparisons demonstrate the close alignment between the collected demos and real-world behaviors.
<div style="display: flex; justify-content: space-between; align-items: center;">
  <img src="../assets/franka/offline_images.gif" alt="Viola Dataset Demo" style="width: 49%; margin-right: 2%;">
  <img src="../assets/franka/real_demo_1.gif" alt="Real Demo" style="width: 49%;">
</div>


### Demonstrations from Simulation
In the second part of our demonstrations, we generated a demo from RLBench which normally uses joint states as the action space. We converted these actions to relative inverse kinematic actions and ran them on the robot. As you can see, the observation space of the robot consists of two images: front and wrist images, providing comprehensive visual feedback on the robot's interactions.

<div style="display: flex; justify-content: space-between;">
  <img src="../assets/franka/rlbench_demo_front_0.gif" alt="RLBench Front Camera" style="width: 24%; margin-right: 1%;">
  <img src="../assets/franka/rlbench_demo_wrist_0.gif" alt="RLBench Wrist Camera" style="width: 24%; margin-right: 1%;">
  <img src="../assets/franka/real_env_demo_front_0.gif" alt="Real World Front Camera" style="width: 24%; margin-right: 1%;">
  <img src="../assets/franka/real_env_demo_wrist_0.gif" alt="Real World Wrist Camera" style="width: 24%;">
</div>