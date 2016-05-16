---
layout: page
title: tags
---
<ul>
{% for post in site.posts %}
{% for tag in post.tags %}
{% if tag == page.tag %}

<li itemprop="name" itemprop=name>{{ post.title }}</li>

{% endif %}
{% endfor %}
{% endfor %}
</ul>
