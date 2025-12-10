---
layout: post
title: "Exploring Multi-Agent Reinforcement Learning: Cooperation, Competition, and Scalability"
date: 2025-11-20
tags: ["reinforcement-learning", "multi-agent", "ml-systems"]
summary: "My first multi-agent RL project and how it connects learning dynamics with system-level concerns."
category: blog
permalink: /blog/multi-agent-rl/
---

Reinforcement Learning (RL) was one of the most conceptually exciting parts of my MSc. For my coursework project, I built a simple **multi-agent RL** environment and implemented tabular Q-learning to explore cooperation and competition between agents.

The setup involved:

- A grid-world environment.
- Two agents with individual rewards.
- Configurable reward structures for cooperative vs competitive tasks.
- Epsilon-greedy exploration and decaying exploration schedules.

Some key observations:

- Early exploration strongly influences the final policy; small changes can lead to very different behaviours.
- Reward shaping can encourage cooperation or fuel competition.
- In competitive scenarios, convergence is slower and less stable.
- Even with simple tabular methods, non-trivial dynamics emerge between agents.

Beyond the algorithmic side, this project sparked system-level questions that align with the ML-Systems perspective:

- How do we scale RL to more agents and more complex environments?
- What happens to training time and stability as we increase parallelism?
- How do resource constraints (compute, memory, communication) shape what is practically achievable?

This project represents my current frontier: connecting **learning dynamics** in RL with **systems considerations** such as distributed training, resource allocation, and scalability. It has reinforced my desire to pursue research in Machine Learning Systems, where these two worlds explicitly intersect.
