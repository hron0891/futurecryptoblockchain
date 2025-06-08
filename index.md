---
layout: home
title: Future Crypto & Blockchain
---

Explore all the latest in DeFi, Web3 and more.

<ul>
  {% for post in paginator.posts %}
    <li><a href="{{ post.url }}">{{ post.title }}</a></li>
  {% endfor %}
</ul>

<div class="pagination">
  {% if paginator.previous_page %}
    <a href="{{ paginator.previous_page_path }}">← Previous</a>
  {% endif %}

  {% if paginator.next_page %}
    <a href="{{ paginator.next_page_path }}">Next →</a>
  {% endif %}
</div>
