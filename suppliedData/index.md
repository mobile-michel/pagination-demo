---
title: Supplied Data
override:tags: [primary]
---
{% for items in collections.supplieddata %}
- [{{ items.data.title }}]({{ items.url | url }})
{% endfor %}