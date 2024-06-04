---
title: Pagination
override:tags: [primary, footer]
---
{% for items in collections.pagination %}
- [{{ items.data.title }}]({{ items.url | url }})
{% endfor %}