---
layout: default
title: Digital & Public
---

# Digital & Public

{% for post in site.posts %}
### [{{ post.title }}]({{ post.url | relative_url }})
<small>{{ post.date | date: "%B %-d, %Y" }}{% if post.lang == "es" %} · Español{% endif %}</small>

{{ post.content | split: '</h1>' | last | split: '</p>' | slice: 0, 2 | join: '</p>' }}</p>

[Read more →]({{ post.url | relative_url }})

---
{% endfor %}

## About the author

Ruth del Campo is a technologist and policy specialist focused on data governance and digital transformation in the public sector. Previously Director of Data for the Government of Spain, she works at the intersection of regulation, technology, and institutional reform.

This blog is one of her personal projects to push beyond her current knowledge with AI. After many years away from code, she is back to building — thanks to tools like Claude Code that make it possible to go from idea to working product in hours, not months. It turns out that a product management background — scoping problems, prioritizing ruthlessly, thinking in systems — is exactly what you need to work effectively with AI. The tools have changed. The discipline hasn't.

It's a genuinely exciting time to be building again.

[More about me →]({{ "/about/" | relative_url }})
