---
layout: page
title: tags
---
{% if site.tags[page.tag] %}
    {% for post in site.tags[page.tag] %}
        <a href="{{ post.url }}/">{{ post.title }}</a>
    {% endfor %}
{% else %}
    <p>There are no posts for this tag.</p>
{% endif %}
