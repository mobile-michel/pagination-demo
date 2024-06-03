---
title: Basic
override:tags: [primary]
---
{% for items in collections.basic %}
- [{{ items.data.title }}]({{ items.url }})
{% endfor %}