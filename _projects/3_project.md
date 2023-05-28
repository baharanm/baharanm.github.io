---
layout: page
title: Robustness agains Data Poisoning Attacks
description: Robust traing against data poisoning
img: assets/img/attack.png
# redirect: assets/img/attack.png
importance: 3
category: work
---

Big datasets empower modern over-parameterized deep learning systems. Such datasets are often scraped from the internet or other public and user-provided sources. An adversary can easily insert a subset of malicious examples into the data collected from public sources to harm the model’s behavior at test time. As a result, deep learning systems trained on public data are extremely vulnerable to data poisoning attacks. Such attacks modify a subset of training examples under small (and potentially invisible) adversarial perturbations, with the aim of changing the model’s prediction on specific
test-time examples. Powerful attacks generate poisons that visually look innocent and are seemingly properly labeled. This makes them hard to detect even by expert observers. Hence, data poisoning attacks are arguably one of the most concerning threats to modern deep learning systems.

We develop powerful defense methods to traing neural networks robust against data poisoning attacks. We consider this problem in supervised setting as well as multimodal language-image pretraining.

Checkout the following papers to know more:

- [Not All Poisons are Created Equal: Robust Training against Data Poisoning](/assets/pdf/yang22poisons_long), ICML 2022

- [Friendly Noise against Adversarial Noise: A Powerful Defense against Data Poisoning Attacks](/assets/pdf/liu22friendly_long.pdf), NeurIPS 2022

- [Robust Contrastive Language-Image Pretraining against Data Poisoning and Backdoor Attacks](https://arxiv.org/pdf/2303.06854), ArXiv Preprint, 2022
