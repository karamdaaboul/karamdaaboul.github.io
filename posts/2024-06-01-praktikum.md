---
layout: post
title: "Group Work Overview"
date: 2024-06-01
categories: Group Work
excerpt: "A brief summary of the group work focusing on key discussions and findings..."
---

## Overview
This page provides summaries of various projects and research works conducted by our group. Each summary is followed by a link to the full document for those interested in more detailed information.

## Categories
- [Robotic Manipulation](#robotic-manipulation)
- [Reinforcement Learning](#reinforcement-learning)

## Group Projects

### Robotic Manipulation
<div id="robotic-manipulation"></div>

#### Project: Investigating the Strengths and Shortcomings of the RT-X Model in Robotic Manipulation (2024, german)
**Summary**: This project investigates the RT-1-X model in the context of robotic manipulation. The foundation model was trained on the Open X-Embodiment dataset. The sudents evaluate the model both in simulated and real environments, using a Franka Panda robot arm, to determine its capabilities and limitations. The RT-1-X model shows solid performance in in-distribution settings but fails to generalize to new, unseen tasks and environments without prior fine-tuning. The study emphasizes the importance of addressing distribution shifts, i.e., the visual differences between training and application environments. Despite the model's promising abilities in familiar scenarios, the investigation highlights the need for further research and development to improve the generalization ability of robotic learning models in diverse real-world applications. [Read the full document](https://github.com/safebotics/safebotics.github.io/blob/master/assets/praktikum_pdf/Investigating_the_Strengths_and_Shortcomings_of_the_RT_X_Model_in_Robotic_Manipulation.pdf){:target="_blank"}

### Reinforcement Learning
<div id="reinforcement-learning"></div>

#### Project: Thinking, Fast and Slow: Application to Reinforcement Learning (2023)
Summary: This paper introduces a novel approach for adapting reinforcement learning algorithms to changes in dynamics during long-term application. Drawing inspiration from Daniel Kahneman's "Thinking, Fast and Slow," the approach equips the reinforcement learning agent with both fast and slow "thinking" systems. Specifically, it combines a Planner and a Soft Actor-Critic (SAC) Policy based on a common Dynamics Model to improve performance during the adaptation phase without compromising long-term reward levels. The paper provides a comprehensive explanation of the approach and presents results from various experiments. Initial results did not meet expectations, but simple adjustments significantly improved performance, suggesting potential for further advancement. [Read the full document](https://github.com/safebotics/safebotics.github.io/blob/master/assets/praktikum_pdf/Thinking__Fast_and_Slow__Application_to_Reinforcement_Learning.pdf){:target="_blank"}