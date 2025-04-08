---
layout: page
title: Blog
subtitle: Thoughts, tutorials, and updates from my journey in tech
---

{% for post in site.posts %}
  <div class="post-preview">
    <a href="{{ post.url | relative_url }}">
      <h2 class="post-title">{{ post.title }}</h2>
      <h3 class="post-subtitle">{{ post.subtitle }}</h3>
    </a>
    <p class="post-meta">Posted on {{ post.date | date: "%B %-d, %Y" }}</p>
    <hr>
  </div>
{% endfor %}
