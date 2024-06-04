---
title: Permalinks
override:tags: [primary, footer]
---
{% for items in collections.permalink %}
- [{{ items.data.title }}]({{ items.url | url }})
{% endfor %}