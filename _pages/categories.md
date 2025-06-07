---
layout: default
title: Categories
permalink: /categories/
---

<section class="categories-list">
  <h1>Categories</h1>
  <ul>
    {% assign sorted_categories = site.categories | sort %}
    {% for category in sorted_categories %}
      {% assign name = category[0] %}
      {% assign posts = category[1] %}
      <li>
        <a href="{{ site.baseurl }}/categories/{{ name | slugify }}/">
          {{ name | capitalize }}
        </a> ({{ posts | size }} post{% if posts.size != 1 %}s{% endif %})
      </li>
    {% endfor %}
  </ul>
</section>
