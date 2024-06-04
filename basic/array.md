---
title: JSON array
description: Uses the array.json data file to iterate over the array of airliners.
date: 2024-02-01
---

There are {{ array.size }} airliners.

{% assign array = array | sort %}
{% for airliner in array %}
- [{{ airliner | capitalize }}]({{ airliner | prepend: '/airliner/' | url }})
  {%- endfor %}

### Structure
{% raw %}
```
{% assign array = array | sort %}
{% for airliner in array %}
- [{{ airliner | capitalize }}]({{ airliner | prepend: '/airliner/' | url }})
{%- endfor %}
```
{% endraw %}