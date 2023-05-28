---
layout: page
title: Low Rank Neural Network Pruning
description: Low Rank Neural Network Pruning
img: assets/img/spurious.png
importance: 3
category: work
---

Neural network pruning is crucial in the face of large, resource-intensive models with billions of parameters. While these models achieve impressive accuracy, they come at a high financial and environmental cost. To address this, we develop pruning methods to reduce over-parameterized networks to smaller ones without compromising test accuracy. Unlike existing methods that simply zero out weights, which cannot realize any training or inference speedup without the use of specialized hardware, our focus lies in approximating weight matrices with low-rank matrices. This approach not only reduces parameters but also enables significant training and inference time speedup on standard hardware, making smaller models more practical for real-world applications like robotics, self-driving cars, and augmented reality.

Checkout the following papers to know more:

- [Low Rank Pruning via Output Perturbation](https://drive.google.com/file/d/1FhuJxrbW554UsMt92WR5B1sCaw8P1odl/view), Sparsity in Neural Netoworks, 2022.
