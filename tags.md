---
layout: page
title: tags
permalink: /tags/
---
<ul>
{% for tag in site.tags %}
  <li>
    <a href="#{{ tag | first | slugize }}">
      {{ tag | first }}
    </a>
  </li>
{% endfor %}
</ul>
