---
layout: page
title: tags
---
<div class = "posts">
<article>
{% for post in site.posts %}
  {% if post.tags contains 'untitled' %}
    <span h1><a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}, {{ post.date | date: '%Y' }}, {{ post.material }}, {{ post.size }}</a></span>
  {% endif  %}
</article>
{% endfor %}
</div>
