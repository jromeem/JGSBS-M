---
layout: default
title: Adventures
permalink: /adventures/
order: 1
---

<div class="home">

  <div class="post-grid row">
    {% for post in site.posts %}
      {% if post.categories contains 'adventures' %}
        <div class="post-tile-contain col-sm-6 col-lg-3">
          <a href="{{ post.url | relative_url }}">
            <div class="post-tile" style="background:url('/assets/images/{{post.tile_bg}}');">
              <p class="post-title">{{ post.title | escape }}</p>
            </div>
          </a>
        </div>
      {% endif %}
    {% endfor %}
  </div>

</div>
