---
layout: page
title: tags
---

<ul>
  {% for tags in page.tags %}
    <li>{{ tags }}</li>
  {% endfor %}
</ul>
