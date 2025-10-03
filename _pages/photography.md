---
layout: page
title: galleries
description: ""
folder: July22nd
permalink: /creative/photography/
nav: false
nav_order: 3
---
{% assign galleries = site.galleries | sort: "importance" %}
<div class="gallery-grid">
  {% for gallery in galleries %}
    {% assign gallery_url = site.baseurl | append: gallery.url %}
    {% include gallery_card.liquid 
      href=gallery_url
      img=gallery.img 
      alt=gallery.description 
      title=gallery.title 
      description=gallery.description %}
  {% endfor %}
</div>

