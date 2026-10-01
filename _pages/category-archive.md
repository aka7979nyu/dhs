---
title: Writing by category
permalink: /categories/
---

{% for group in site.categories %}
## {{ group[0] }}
{% for post in group[1] %}
- [{{ post.title }}]({{ post.url | relative_url }})
{% endfor %}
{% endfor %}

[Browse all writing]({{ '/posts/' | relative_url }}).
