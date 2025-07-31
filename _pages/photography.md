---
layout: page
title: photography
description: "trying out a new hobby :)"
folder: July22nd
permalink: /creative/photography/
nav: false
nav_order: 3
---
{% assign galleries = site.galleries | sort: "importance" %}
<div class="gallery-grid">
  {% for gallery in galleries %}
    {% include gallery_card.liquid 
      href=gallery.url 
      img=gallery.img 
      alt=gallery.description 
      title=gallery.title 
      description=gallery.description %}
  {% endfor %}
</div>
