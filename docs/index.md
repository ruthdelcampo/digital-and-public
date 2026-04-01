---
layout: default
title: Digital & Public
---

# Digital & Public

{% for post in site.posts %}
### [{{ post.title }}]({{ post.url | relative_url }})
<small>{{ post.date | date: "%B %-d, %Y" }}{% if post.lang == "es" %} · Español{% endif %}</small>

{{ post.content | split: '</p>' | slice: 0, 2 | join: '</p>' }}</p>

[Read more →]({{ post.url | relative_url }})

---
{% endfor %}
