---
title: Test variables
description:
layout: default
tags: [primary, supplieddata]
date: 2024-01-01
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
