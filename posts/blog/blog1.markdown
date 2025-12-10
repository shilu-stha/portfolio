---
layout: post
title: "Understanding Gradient Descent: Intuition Beyond the Equations"
date: 2024-06-02
tags: ["machine-learning", "optimisation", "gradient-descent"]
summary: "A practical, intuition-first walkthrough of gradient descent and its role in training modern ML models."
category: blog
permalink: /blog/gradient-descent-intuition/
---

Gradient descent is the workhorse behind many machine learning algorithms. It’s easy to memorise the update rule, but understanding the **behaviour** of gradient descent is much more valuable than just knowing the formula.

At its core, gradient descent is a search strategy:

1. Compute how the loss changes with respect to each parameter.
2. Move in the direction that reduces the loss the most (the negative gradient).
3. Repeat until changes become small or performance plateaus.

During my MSc, I implemented several variants from scratch:

- **Batch Gradient Descent**: Uses the full dataset each step; stable but slow.
- **Stochastic Gradient Descent (SGD)**: Updates per sample; noisy but often finds minima that generalise better.
- **Mini-batch Gradient Descent**: A balance between the two and the de facto standard in deep learning.

I experimented with different learning rates and saw firsthand how:

- Too large a learning rate leads to divergence or oscillation.
- Too small leads to painfully slow convergence.
- Schedules (step decay, cosine, etc.) can significantly improve training.

These experiments helped me see why optimisers like Adam, RMSProp, and momentum methods exist: they adapt the step size and direction using history, making training more robust to poorly scaled gradients.

For someone coming from a systems and engineering background, gradient descent feels like an iterative feedback loop: measure, adjust, repeat. That mental model has helped me reason about both ML training and optimisation problems in other domains.
