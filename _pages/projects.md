---
layout: page
title: Projects
permalink: /projects/
# description: <h6>We aim to address <b>sustainability, reliability, and efficiency</b> of machine learning, by selecting the most relevant data for training, among other techniques.</h6>
nav: true
nav_order: 2
display_categories: [efficiency, robustness]
horizontal: false
---
<!-- We aim to address <span class="emp"><b>sustainability, reliability, and efficiency</b></span> of machine learning, by selecting the most relevant data for training, among other techniques. -->

We aim to address [sustainability and efficiency](#efficiency), as well as [reliability and robustness](#robustness) of learning from large datasets. Our research mainly focuses on addressing the above problems by selecting the most relevant data for training. But we also work on finding better models and developing better training methods.


<!-- pages/projects.md -->
<div class="projects">
{%- if site.enable_project_categories and page.display_categories %}
  <!-- Display categorized projects -->
  {%- for category in page.display_categories %}
  {%- if category == 'efficiency' %}
    <a id="efficiency"></a>
  {%- endif -%}
  {%- if category == 'robustness' %}
    <a id="robustness"></a>
  {%- endif -%}
  <h2 class="category">{{ category }}</h2>
  {%- assign categorized_projects = site.projects | where: "category", category -%}
  {%- assign sorted_projects = categorized_projects | sort: "importance" %}
  <!-- Generate cards for each project -->
  {% if page.horizontal -%}
  <div class="container">
    <div class="row row-cols-2">
    {%- for project in sorted_projects -%}
      {% include projects_horizontal.html %}
    {%- endfor %}
    </div>
  </div>
  {%- else -%}
  <div class="grid">
    {%- for project in sorted_projects -%}
      {% include projects.html %}
    {%- endfor %}
  </div>
  {%- endif -%}
  {% endfor %}

{%- else -%}
<!-- Display projects without categories -->
  {%- assign sorted_projects = site.projects | sort: "importance" -%}
  <!-- Generate cards for each project -->
  {% if page.horizontal -%}
  <div class="container">
    <div class="row row-cols-2">
    {%- for project in sorted_projects -%}
      {% include projects_horizontal.html %}
    {%- endfor %}
    </div>
  </div>
  {%- else -%}
  <div class="grid">
    {%- for project in sorted_projects -%}
      {% include projects.html %}
    {%- endfor %}
  </div>
  {%- endif -%}
{%- endif -%}
</div>
