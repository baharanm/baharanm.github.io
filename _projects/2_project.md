---
layout: page
title: Robustness against Label Noise
description: Robust Training against Label Noise
img: assets/img/noise.png
importance: 2
category: work
---

The success of deep neural networks relies heavily on the quality of training data, and in particular accurate labels of the training examples. However, maintaining label quality becomes very expensive for large datasets, and hence mislabeled data points are ubiquitous in large real-world datasets. As deep neural networks have the capacity to essentially memorize any (even random) labeling of the data, noisy labels have a drastic effect on the generalization performance of deep neural networks. Therefore, it becomes crucial to develop methods with strong theoretical guarantees for robust training of neural networks against noisy labels. Such guarantees become of the utmost importance in safety-critical systems, such as aircraft, autonomous cars, and medical devices.

We develop principled techniques with strong theoretical guarantees for robust training of neural networks against noisy labels. We consider the effect of data, model, and pretraining on robustness against label noise.

Checkout the following papers to know more:

- [Investigating Why Contrastive Learning Benefits Robustness Against Label Noise](/assets/pdf/xue22investigating_long.pdf), ICML 2022

- [The Final Ascent: When Bigger Models Generalize Worse on Noisy-labeled Data](https://arxiv.org/pdf/2208.08003.pdf), ArXiv Preprint 2022

- [Coresets for Robust Training of Neural Networks against Noisy Labels](/assets/pdf/mirzasoleiman20coresetslong.pdf), NeurIPS 2020
