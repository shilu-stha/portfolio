---
layout: post
title: "Building Convolutional Neural Networks from Scratch"
date: 2025-03-21
tags: ["deep-learning", "cnn", "computer-vision"]
summary: "Implementing CNNs layer-by-layer to understand how they learn spatial features."
category: blog
permalink: /blog/building-cnns-from-scratch/
---

Convolutional Neural Networks (CNNs) are a staple of modern computer vision. To move beyond high-level diagrams, I built small CNNs from scratch using NumPy, implementing:

- Convolutional layers
- Padding and stride
- Max-pooling
- Non-linear activations
- Backpropagation through all of the above

I trained a simple CNN on a subset of CIFAR-10 and experimented with:

- Different kernel sizes
- Varying network depth
- ReLU vs Leaky ReLU activations
- Basic data augmentation (flips, crops, normalisation)

Some practical lessons:

- **Depth vs performance**: Deeper isn’t always better; capacity must match data.
- **Data augmentation** often matters more than increasing model size.
- **Initialisation** heavily influences training stability.
- **Batch normalisation** can dramatically accelerate and stabilise training.

Visualising feature maps helped me see what the network was learning: early layers detected edges and simple patterns, while later layers responded to more complex shapes.

For someone with a strong engineering background, treating CNNs as systems composed of modules—each transforming the data in specific ways—made them much more intuitive. This mindset carries over naturally into thinking about **ML systems as whole pipelines**, not just standalone models.
