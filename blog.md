---
layout: page
title: Blog
permalink: /blog/
---

# Blog Posts

<ul>
  {% for post in site.posts %}
    <li>
      <h3><a href="{{ post.url }}">{{ post.title }}</a></h3>
      <span>{{ post.date | date: "%B %-d, %Y" }}</span>
      {% if post.excerpt %}
        <p>{{ post.excerpt }}</p>
      {% endif %}
    </li>
  {% endfor %}
</ul>