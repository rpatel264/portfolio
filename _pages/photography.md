---
layout: page
title: photography
permalink: /creative/photography/
description:
nav: false
nav_order: 3
display_categories: [2024, 2023]  # Optional: update as needed
horizontal: false
---

<!-- pages/photography.md -->
<div class="projects">
{% if site.enable_project_categories and page.display_categories %}
  <!-- Display categorized galleries -->
  {% for category in page.display_categories %}
  <a id="{{ category }}" href=".#{{ category }}">
    <h2 class="category">{{ category }}</h2>
  </a>
  {% assign categorized_galleries = site.galleries | where: "category", category %}
  {% assign sorted_galleries = categorized_galleries | sort: "importance" %}
  <!-- Generate cards for each gallery -->
  {% if page.horizontal %}
  <div class="container">
    <div class="row row-cols-1 row-cols-md-2">
    {% for gallery in sorted_galleries %}
      {% include projects_horizontal.liquid project=gallery %}
    {% endfor %}
    </div>
  </div>
  {% else %}
  <div class="row row-cols-1 row-cols-md-3">
    {% for gallery in sorted_galleries %}
      {% include projects.liquid project=gallery %}
    {% endfor %}
  </div>
  {% endif %}
  {% endfor %}

{% else %}

<!-- Display galleries without categories -->
{% assign sorted_galleries = site.galleries | sort: "importance" %}

{% if page.horizontal %}
  <div class="container">
    <div class="row row-cols-1 row-cols-md-2">
    {% for gallery in sorted_galleries %}
      {% include projects_horizontal.liquid project=gallery %}
    {% endfor %}
    </div>
  </div>
{% else %}
  <div class="row row-cols-1 row-cols-md-3">
    {% for gallery in sorted_galleries %}
      {% include projects.liquid project=gallery %}
    {% endfor %}
  </div>
{% endif %}

{% endif %}
</div>
