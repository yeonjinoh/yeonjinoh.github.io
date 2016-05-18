---
layout: page
title: tags
---


<div id="tags">
  <ul class="tag-box inline">
  {% for item in (0..site.tags.size) %}{% unless forloop.last %}
    {% capture this_word %}{{ tag_words[item] | strip_newlines }}{% endcapture %}
    <li><a href="#{{ this_word | cgi_escape }}">{{ this_word }} <span>{{ site.tags[this_word].size }}</span></a></li>
  {% endunless %}{% endfor %}
  </ul>

  {% for item in (0..site.tags.size) %}{% unless forloop.last %}
    {% capture this_word %}{{ tag_words[item] | strip_newlines }}{% endcapture %}
  <h2 id="{{ this_word | cgi_escape }}">{{ this_word }}</h2>
  <ul class="posts">
    {% for post in site.tags[this_word] %}{% if post.title != null %}
    <li itemscope><span class="entry-date"><time datetime="{{ post.date | date_to_xmlschema }}" itemprop="datePublished">{{ post.date | date: "%B %d, %Y" }}</time></span> &raquo; <a href="{{ post.url }}">{{ post.title }}</a></li>
    {% endif %}{% endfor %}
  </ul>
  {% endunless %}{% endfor %}
</div>


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
