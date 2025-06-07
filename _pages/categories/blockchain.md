---
title: "Blockchain Technology & Use Cases"
layout: category
permalink: /categories/blockchain/
category: blockchain
parent: Categories
description: "Explore the future of blockchain across industries including supply chain, healthcare, and public infrastructure."
author_profile: false
---


<ul>
  {% assign posts_in_category = site.posts | where_exp: "post", "post.categories contains 'blockchain'" %}
  {% for post in posts_in_category %}
    <li><a href="{{ post.url | relative_url }}">{{ post.title }}</a> — {{ post.date | date: "%B %d, %Y" }}</li>
  {% endfor %}
</ul>
