---
layout: page
title: test
---

<div id="title">
  {% assign thistagssize = page.tags | size %}
      {% for post in site.posts %} <!-- 포스트 전체 리스트를 호출한다 -->
        {% if thistagssize == 1 %}
          {% if post.tags contains page.tags[0] %} <!-- 호출된 포스트 리스트 중 현재 포스트의 태그가 포함된 포스트를 걸러낸다 -->
          <h1><a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}, {{ post.date | date: '%Y' }}, {{ post.material }}, {{ post.size }}</a></h1>
          {% endif %}
        {% endif  %}
      {% endfor %}
</div>
