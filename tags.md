---
layout: page
title: tags
---
<div class = "posts">
<!--parkingspot section-->
<article>
    {% for post in site.posts %} <!-- 포스트 전체 리스트를 호출한다 -->
      {% if post.tags contains 'parkingspot' %} <!-- 호출된 포스트 리스트 중 'parkingspot' 태그가 포함된 포스트를 걸러낸다 -->
        <h1><a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}, {{ post.date | date: '%Y' }}, {{ post.material }}, {{ post.size }}</a></h1>
      {% endif  %}
    {% endfor %}
</article>

<!--stairs section-->
<article>
    {% for post in site.posts %}
      {% if post.tags contains 'stairs' %}
        <h1><a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}, {{ post.date | date: '%Y' }}, {{ post.material }}, {{ post.size }}</a></h1>
      {% endif  %}
    {% endfor %}
</article>

<!--cross section-->
<article>
    {% for post in site.posts %}
      {% if post.tags contains 'cross' %}
        <h1><a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}, {{ post.date | date: '%Y' }}, {{ post.material }}, {{ post.size }}</a></h1>
      {% endif  %}
    {% endfor %}
</article>

<!--cube section-->
<article>
    {% for post in site.posts %}
      {% if post.tags contains 'cube' %}
        <h1><a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}, {{ post.date | date: '%Y' }}, {{ post.material }}, {{ post.size }}</a></h1>
      {% endif  %}
    {% endfor %}
</article>

<!--building section-->
<article>
    {% for post in site.posts %}
      {% if post.tags contains 'building' %}
        <h1><a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}, {{ post.date | date: '%Y' }}, {{ post.material }}, {{ post.size }}</a></h1>
      {% endif  %}
    {% endfor %}
</article>

<!--playground section-->
<article>
    {% for post in site.posts %}
      {% if post.tags contains 'playground' %}
        <h1><a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}, {{ post.date | date: '%Y' }}, {{ post.material }}, {{ post.size }}</a></h1>
      {% endif  %}
    {% endfor %}
</article>

<!--puppy section-->
<article>
    {% for post in site.posts %}
      {% if post.tags contains 'puppy' %}
        <h1><a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}, {{ post.date | date: '%Y' }}, {{ post.material }}, {{ post.size }}</a></h1>
      {% endif  %}
    {% endfor %}
</article>

<!--grid section-->
<article>
    {% for post in site.posts %}
      {% if post.tags contains 'grid' %}
        <h1><a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}, {{ post.date | date: '%Y' }}, {{ post.material }}, {{ post.size }}</a></h1>
      {% endif  %}
    {% endfor %}
</article>

<!--trapezoid section-->
<article>
    {% for post in site.posts %}
      {% if post.tags contains 'trapezoid' %}
        <h1><a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}, {{ post.date | date: '%Y' }}, {{ post.material }}, {{ post.size }}</a></h1>
      {% endif  %}
    {% endfor %}
</article>

<!--edges section-->
<article>
    {% for post in site.posts %}
      {% if post.tags contains 'edges' %}
        <h1><a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}, {{ post.date | date: '%Y' }}, {{ post.material }}, {{ post.size }}</a></h1>
      {% endif  %}
    {% endfor %}
</article>

<!--woman section-->
<article>
    {% for post in site.posts %}
      {% if post.tags contains 'woman' %}
        <h1><a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}, {{ post.date | date: '%Y' }}, {{ post.material }}, {{ post.size }}</a></h1>
      {% endif  %}
    {% endfor %}
</article>

<!--Color-Index-#2 section-->
<article>
    {% for post in site.posts %}
      {% if post.tags contains 'Color-Index-#2' %}
        <h1><a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}, {{ post.date | date: '%Y' }}, {{ post.material }}, {{ post.size }}</a></h1>
      {% endif  %}
    {% endfor %}
</article>

<!--stairs section-->
<article>
    {% for post in site.posts %}
      {% if post.tags contains 'Color-Index-#1' %}
        <h1><a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}, {{ post.date | date: '%Y' }}, {{ post.material }}, {{ post.size }}</a></h1>
      {% endif  %}
    {% endfor %}
</article>

<!--untitled section-->
<article>
    {% for post in site.posts %}
      {% if post.tags contains 'untitled' %}
        <h1><a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}, {{ post.date | date: '%Y' }}, {{ post.material }}, {{ post.size }}</a></h1>
      {% endif  %}
    {% endfor %}
</article>

<!--nightscape section-->
<article>
    {% for post in site.posts %}
      {% if post.tags contains [nightscape, square]  %}
        <h1><a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}, {{ post.date | date: '%Y' }}, {{ post.material }}, {{ post.size }}</a></h1>
      {% endif  %}
    {% endfor %}
</article>

<!--nightscape section-->
<article>
    {% for post in site.posts %}
      {% if post.tags contains [nightscape, landscape] %}
        <h1><a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}, {{ post.date | date: '%Y' }}, {{ post.material }}, {{ post.size }}</a></h1>
      {% endif  %}
    {% endfor %}
</article>

<!--still mute section-->
<article>
    {% for post in site.posts %}
      {% if post.tags contains 'still-mute' %}
        <h1><a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}, {{ post.date | date: '%Y' }}, {{ post.material }}, {{ post.size }}</a></h1>
      {% endif  %}
    {% endfor %}
</article>
</div>
