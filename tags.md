---
layout: page
title: tags
---
<ul>
{% for tag in site.tags | sort %}
  <li>
    <a href="#{{ tag | first | slugize }}">
      {{ tag | first }}
    </a>
  </li>
{% endfor %}
</ul>
