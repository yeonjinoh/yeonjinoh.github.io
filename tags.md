---
layout: page
title: tags
---

{% for post in site.posts %}
  {% if post.tags contains 'untitled' %}
    <h1><a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}, {{ post.date | date: '%Y' }}, {{ post.material }}, {{ post.size }}</a></h1>
  {% endif  %}
{% endfor %}
