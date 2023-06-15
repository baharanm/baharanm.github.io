---
layout: page
title: Data Poisoning
description: Robust traing against data poisoning
img: assets/img/projects/poison_project.png
# redirect: assets/img/attack.png
importance: 3
category: robustness
---

Big datasets empower modern over-parameterized deep learning systems. Such datasets are often scraped from the internet or other public and user-provided sources. An adversary can easily insert a subset of malicious examples into the data collected from public sources to harm the model’s behavior at test time. As a result, deep learning systems trained on public data are extremely vulnerable to data poisoning attacks. Such attacks modify a subset of training examples under small (and potentially invisible) adversarial perturbations, with the aim of changing the model’s prediction on specific
test-time examples. Powerful attacks generate poisons that visually look innocent and are seemingly properly labeled. This makes them hard to detect even by expert observers. Hence, data poisoning attacks are arguably one of the most concerning threats to modern deep learning systems.

We develop powerful defense methods to traing neural networks robust against data poisoning attacks. We consider this problem in supervised setting as well as multimodal language-image pretraining.

<div class="row justify-content-sm-center">
	<div class="col-sm-8 mt-3 mt-md-0">
	    {% include figure.html path="assets/img/projects/poison.png" title="poison" class="img-fluid rounded z-depth-1" %}
	</div>
</div>
<!-- <div class="caption">
    This image can also have a caption. It's like magic.
</div> -->

Checkout the following papers to know more:

<div class="publications">
{% bibliography -f {{ site.scholar.bibliography }} -q @*[poison=true]* %}
</div>
