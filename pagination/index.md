---
title: Pagination
override:tags: [primary]
---
{% for items in collections.pagination %}
- [{{ items.data.title }}]({{ items.url }})
{% endfor %}