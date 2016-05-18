---
layout: page
title: tags
---
<article>
{% for post in site.posts %}
  {% if post.tags contains 'untitled' %}
    <a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}, {{ post.date | date: '%Y' }}, {{ post.material }}, {{ post.size }}</a>
  {% endif  %}
{% endfor %}
</article>
