---
layout: default
title: Blog
---

{% for post in site.posts %}
## [{{ post.title }}]({{ post.url }})

{{ post.content }}

<hr class="nice-hr">
{% endfor %}
