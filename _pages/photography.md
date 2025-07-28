---
layout: page
title: Photography Gallery
permalink: /creative/photography/
nav: false
---

# Photography Galleries

<div class="gallery">
  {% for photo in site.data.photos %}
    <a href="{{ '/assets/img/photography/' | append: photo | relative_url }}" target="_blank" rel="noopener noreferrer">
      <img src="{{ '/assets/img/photography/' | append: photo | relative_url }}" alt="Photo {{ forloop.index }}" />
    </a>
  {% endfor %}
</div>

<style>
  .gallery {
    display: flex;
    flex-wrap: wrap;
    gap: 12px;
    justify-content: center;
  }
  .gallery img {
    max-width: 300px;
    border-radius: 6px;
    cursor: pointer;
    transition: transform 0.2s ease;
  }
  .gallery img:hover {
    transform: scale(1.05);
  }
</style>
