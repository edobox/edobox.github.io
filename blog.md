---
layout: page
title: Blog
---

## 📝 Blog

{% if site.posts.size > 0 %}
<ul>
  {% for post in site.posts %}
    <li>
      <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
      <span style="color:#888;font-size:0.9em;">({{ post.date | date: '%b %d, %Y' }})</span>
    </li>
  {% endfor %}
</ul>
{% else %}
<p>No posts available yet. Check back soon!</p>
{% endif %}