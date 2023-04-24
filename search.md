---
layout: default
title: Search Results
---

<h1>Search Results for "{{ page.query }}"</h1>

<ul>
{% for post in site.posts %}
  {% if post.content contains page.query %}
    <li><a href="{{ post.url }}">{{ post.title }}</a></li>
  {% endif %}
{% endfor %}
</ul>
