---
layout: page
title: tags
---
<div class = "posts">
<article>
    {% for post in site.posts %}
      <section>
      {% if post.tags contains 'untitled' %}
        <h1><a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}, {{ post.date | date: '%Y' }}, {{ post.material }}, {{ post.size }}</a></h1>
      {% endif  %}
      </section>
    {% endfor %}
</article>
</div>
