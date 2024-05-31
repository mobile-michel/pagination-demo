---
title: Permalinks
override:tags: [primary]
---
{% for items in collections.permalink %}
- [{{ items.data.title }}]({{ items.url }})
{% endfor %}