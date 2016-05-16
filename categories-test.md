---
layout: page
title: categories
---
    {% if site.category[page.category] %}
        {% for post in site.category[page.category] %}
            <a href="{{ post.url }}/">{{ post.title }}</a>
        {% endfor %}
    {% else %}
        <p>There are no posts for this tag.</p>
    {% endif %}
