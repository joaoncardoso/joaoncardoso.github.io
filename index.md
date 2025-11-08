---
layout: default
title: Home
---

# Welcome to My Website

Hello! I'm [Your Name], and this is my personal website.

## What You'll Find Here

- **[About Me](/about)** - Learn more about my background and interests
- **[CV](/cv)** - My professional experience and qualifications
- **[Blog](/blog)** - Thoughts, tutorials, and updates
- **[Contact](/contact)** - Get in touch with me

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