---
layout: page
title: Label Noise
description: Robust traing against label nosie
img: assets/img/projects/noise_project.png
importance: 2
category: robustness
---

The success of deep neural networks relies heavily on the quality of training data, and in particular accurate labels of the training examples. However, maintaining label quality becomes very expensive for large datasets, and hence mislabeled data points are ubiquitous in large real-world datasets. As deep neural networks have the capacity to essentially memorize any (even random) labeling of the data, noisy labels have a drastic effect on the generalization performance of deep neural networks. Therefore, it becomes crucial to develop methods with strong theoretical guarantees for robust training of neural networks against noisy labels. Such guarantees become of the utmost importance in safety-critical systems, such as aircraft, autonomous cars, and medical devices.

We develop principled techniques with strong theoretical guarantees for robust training of neural networks against noisy labels. We consider the effect of data, model, and pretraining on robustness against label noise.

<div class="row justify-content-sm-center">
	<div class="col-sm-12 mt-3 mt-md-0">
	    {% include figure.html path="assets/img/projects/label_noise.png" title="label noise" class="img-fluid rounded z-depth-1" %}
	</div>
</div>
<div class="caption">
    Examples of Noisy Labels. Source: https://arxiv.org/pdf/1711.00583v1.pdf
</div>

Checkout the following papers to know more:

<div class="publications">
{% bibliography -f {{ site.scholar.bibliography }} -q @*[noise=true]* %}
</div>

