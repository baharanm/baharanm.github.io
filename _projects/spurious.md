---
layout: page
title: Spurious Correlations
description: Robust traing against spurious correlations
img: assets/img/projects/spurious.png
importance: 3
category: robustness
---

<!-- Spurious correlations that degrade model generalization or lead the model to be right for the wrong reasons are one of the main robustness concerns for real-world deployments.  -->

Neural networks are known to exploit spurious correlations in the training data: certain attributes that may correlate with certain categories during training, but are not predictive of the categories in general. For example, if the majority of lighter images co-occur with flame, the model may learn to associate the flame with the lighter category, rather than relying on the lighter to make the prediction. Similarly, a toxicity classifier may learn to spuriously associate toxicity with the mention of certain demographics in the text. Such biases degrade models’ worst-group test performance on minority groups that do not exhibit the spurious correlation.

We develop methods to mitigate the effect of spurious correlations during training neural networks. We consider robust training in supervised scenario, and mitigating spurious correlations from supervised or multimodal pretrained models during fine-tuning.

<div class="row justify-content-sm-center">
	<div class="col-sm-10 mt-3 mt-md-0">
	    {% include figure.html path="assets/img/projects/spurious_in.png" title="spurious" class="img-fluid rounded z-depth-1" %}
	</div>
</div>
<!-- <div class="caption">
    This image can also have a caption. It's like magic.
</div> -->

Checkout the following papers to know more:

<div class="publications">
{% bibliography -f {{ site.scholar.bibliography }} -q @*[spurious=true]* %}
</div>