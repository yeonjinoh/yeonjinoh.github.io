---
layout: page
title: tags
---
{% for post in posts %}
  {% if post.tags contains "mdf" %}
    <a href="{{ post.url }}">{{ post.title }}</a>
  {% endif %}
{% endfor %}
