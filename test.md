---
title: Test variables
layout: default
tags: [primary, supplieddata]
date: 2024-12-01
---

{% for item in collections.airliner %}

- {{ item.data.title }}
  {% endfor %}

#### Structure

```
<ul>
  {%- raw %}
  {% for item in collections.airliner %}
  <li>{{ item.data.title }}</li>
  {% endfor %}
{% endraw -%}
</ul>
```
