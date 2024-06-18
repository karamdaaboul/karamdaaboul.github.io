---
layout: post
title: "Softwares Overview"
date: 2024-06-01
categories: Softwares
excerpt: "A brief summary of the softwares focusing on key discussions and findings..."
---

## Softwares
- [GymPanda RL Studio](#gympanda-rl-studio)
- [Safety Isaac Orbit/Lab](#safety-isaac)

## GymPanda RL Studio
<div id="gympanda-rl-studio"></div>

**GymPanda RL Studio** is a straightforward software framework tailored for managing the [Franka Panda robot](https://franka.de/de/) using simple reinforcement learning techniques. This software allows users to explore different action spaces, from relative to absolute gripper positions, and supports various observation spaces, including pixel-based or state-based measurements. The designed environments are compatible with reinforcement learning frameworks like [Stable Baselines 3](https://github.com/DLR-RM/stable-baselines3). Additionally, the software is designed to be used without prior knowledge of [ROS](https://www.ros.org/), simplifying the learning curve for new users.


<img src="../assets/franka/franka_gym.svg" alt="Franka KIT Overview" style="width: 600px; height: auto;"> 

### GymPanda RL Studio Features

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
In the first part of our demonstrations, we utilized an episode from the [Viola dataset](https://www.tensorflow.org/datasets/catalog/viola) and implemented it on a real robot. The visual comparisons demonstrate the close alignment between the demonstrations collected from the dataset and the real-world behaviors observed.
<div style="display: flex; justify-content: space-between; align-items: center;">
  <img src="../assets/franka/offline_images.gif" alt="Viola Dataset Demo" style="width: 49%; margin-right: 2%;">
  <img src="../assets/franka/real_demo_1.gif" alt="Real Demo" style="width: 49%;">
</div>

### Demonstrations from Simulation
In the second part of our demonstrations, we generated a demo from [RLBench](https://sites.google.com/view/rlbench), which normally uses joint states as the action space. We converted these actions into relative inverse kinematic actions for execution on the robot. The observation space includes front and wrist camera views, providing comprehensive visual feedback on the robot’s interactions.
<div style="display: flex; justify-content: space-between;">
  <img src="../assets/franka/rlbench_demo_front_0.gif" alt="RLBench Front Camera" style="width: 24%; margin-right: 1%;">
  <img src="../assets/franka/rlbench_demo_wrist_0.gif" alt="RLBench Wrist Camera" style="width: 24%; margin-right: 1%;">
  <img src="../assets/franka/real_env_demo_front_0.gif" alt="Real World Front Camera" style="width: 24%; margin-right: 1%;">
  <img src="../assets/franka/real_env_demo_wrist_0.gif" alt="Real World Wrist Camera" style="width: 24%;">
</div>

### Using Reinforcement Learning
We trained the agent using a simplified version of the environment through reinforcement learning, where the action space was limited to the position of the gripper. The task was a simple goal-reaching task. Only the front camera's observation was utilized for this training.
<iframe width="560" height="315" src="https://www.youtube.com/embed/MVICOvh-xxY" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>


## Safety Isaac Orbit/Lab
<div id="safety-isaac"></div>
<img src="../assets/safety_orbit/safety_isaac.svg" alt="Safety Isaac Overview" style="width: 400px; height: auto;"> 

<img src="../assets/safety_orbit/safety_orbit.png" alt="example" style="width: 400px; height: auto;"> 