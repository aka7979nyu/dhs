---
title: Writing
permalink: /posts/
---

{% if site.posts.size > 0 %}
{% for post in site.posts %}
## [{{ post.title }}]({{ post.url | relative_url }})
{{ post.date | date: '%B %-d, %Y' }}
{{ post.excerpt }}
{% endfor %}
{% else %}
No course posts have been published yet. The accompanying blog post for the Bahrain map is still to be written.

[Open the published Bahrain map]({{ '/BH_featuremapNEW.html' | relative_url }}).
{% endif %}
