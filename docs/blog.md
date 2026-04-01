---
layout: default
title: Blog
permalink: /blog/
---

# Blog

{% for post in site.posts %}
### [{{ post.title }}]({{ post.url | relative_url }})
<small>{{ post.date | date: "%B %-d, %Y" }}{% if post.lang == "es" %} · Español{% endif %}</small>

{{ post.excerpt }}

---
{% endfor %}
