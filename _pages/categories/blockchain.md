---
title: "Blockchain Technology & Use Cases"
layout: category
permalink: /categories/blockchain/
category: blockchain
parent: Categories
description: "Explore the future of blockchain across industries including supply chain, healthcare, and public infrastructure."
author_profile: false
---

{% assign blockchain_posts = site.posts | where_exp: "post", "post.categories contains 'blockchain'" %}
<ul>
  {% for post in blockchain_posts %}
    <li>
      <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
    </li>
  {% endfor %}
</ul>
