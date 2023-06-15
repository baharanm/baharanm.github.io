---
layout: page
title: Data-efficiency
description: Data-efficient machine learning
img: assets/img/projects/efficient.png
importance: 1
category: efficiency
---

Large datasets have enabled over-parameterized neural networks to achieve unprecedented success. However, training such models, with millions or billions of parameters, on large data requires expensive computational resources, which consume substantial energy, leave a massive amount of carbon footprint, and often soon become obsolete and turn into e-waste. While there has been a persistent effort to improve the performance and reliability of machine learning models, their sustainability is often neglected.

To address the sustainability and efficiency of machine learning, one approach involves selecting the most relevant data for training. We address the above problem by proposing rigorous methods to find coresets for training machine learning models, in particular neural networks. 
<!-- We address this problem both in supervised settings, as well as unsupervised setting for pretraining large models on large datasets. -->

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/projects/efficient_project.png" title="efficient" class="img-fluid rounded z-depth-1" %}
    </div>
</div>

Checkout the following papers to know more:

<div class="publications">
{% bibliography -f {{ site.scholar.bibliography }} -q @*[efficient=true]* %}
</div>




