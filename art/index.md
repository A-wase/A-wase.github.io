---
layout: default
title: Art
---

<h1>Art</h1>

<div class="art-grid">

{% for artwork in site.artwork %}

  <a class="art-item" href="{{ artwork.url | relative_url }}">

    {% if artwork.image %}
      <img src="{{ artwork.image | relative_url }}" alt="{{ artwork.title }}">
    {% endif %}

    <div class="art-title">
      {{ artwork.title }}
    </div>

  </a>

{% endfor %}

</div>