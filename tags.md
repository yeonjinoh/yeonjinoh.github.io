---
layout: page
title: tags
---

{% assign tags = page.tags | split:&nbsp; %}
<ul>
    {% for tag in tags %}
    <li>{{ tag }}</li>
    {% endfor %}
</ul>
