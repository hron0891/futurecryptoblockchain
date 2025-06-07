---
layout: single
title: Categories
permalink: /categories-list/
---

<ul>
  {% assign sorted_categories = site.categories | sort %}
  {% for category in sorted_categories %}
    {% assign name = category[0] %}
    {% assign posts = category[1] %}
    <li>
      <a href="{{ '/categories/' | append: name | slugify | append: '/' | relative_url }}">
        {{ name | capitalize }}
      </a> ({{ posts | size }} post{% if posts.size != 1 %}s{% endif %})
    </li>
  {% endfor %}
</ul>
