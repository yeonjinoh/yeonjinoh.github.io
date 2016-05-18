---
layout: page
title: tags
---


{% for tag in site.tags %}
<ul>
  {% for post in tag | last %}
    {% if post.tags contains 'tilt' %}
  <li>
      <a href="{{ post.url }}">{{ post.title }}</a>
      <span class="date">{{ post.date | date: "%B %-d, %Y"  }}</span>
  </li>
    {% endif %}
  {% endfor %}
{% endfor %}
</ul>


<!--{% for tag in site.tags %}-->
<!--  {% assign tag_first = tag | first %}-->
<!--  {% assign tag_last = tag | last %}-->

<!--{{ tag_first | downcase }}-->
<!--<ul>-->
<!--{% for post in tag_last %}-->
<!--  {% if post.tags contains tag_first %}-->
<!--  <li>-->
<!--    <a href="{{ post.url }}">{{ post.title }}</a>-->
<!--    <span class="date">{{ post.date | date: "%B %-d, %Y"  }}</span>-->
<!--  </li>-->
<!--  {% endif %}-->
<!--{% endfor %}-->
<!--</ul>-->
<!--{% endfor %}-->
