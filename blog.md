---
title: Blog
permalink: /blog/
nav_order: 2
---
Total posts: {{ site.posts.size }}
{% for post in site.posts %}
- [{{ post.title }}]({{ post.url | relative_url }}) — {{ post.date | date: "%Y-%m-%d" }}
{% endfor %}
