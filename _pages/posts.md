---
layout: page
title: Writing
permalink: /posts/
---

# Writing

{% if site.posts.size > 0 %}
  {% for post in site.posts %}
- [{{ post.title }}]({{ post.url | relative_url }})
  {% endfor %}
{% else %}
No posts published yet.
{% endif %}
