---
layout: default
title: Home
---

# Welcome to My Website

Hello! I'm João, and this is my personal website.

## What You'll Find Here

- **[About Me](/about)**
- **[CV](/cv)**
- **[Blog](/blog)**
- **[Contact](/contact)**

## Recent Posts

<ul>
  {% for post in site.posts limit:5 %}
    <li>
      <span>{{ post.date | date: "%b %-d, %Y" }}</span>
      <a href="{{ post.url }}">{{ post.title }}</a>
    </li>
  {% endfor %}
</ul>

[View all posts →](/blog)