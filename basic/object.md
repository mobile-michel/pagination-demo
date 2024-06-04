---
title: JSON objects
description: Uses the object.json data file to iterate over the airliner's objects.
date: 2024-02-02
---
{% assign object = object | sort: 'model' %}
{% for airliner in object %}
- [{{ airliner.company }} {{ airliner.model | capitalize }}]({{ airliner.model | prepend: '/airliner/' | url }})
{%- endfor %}

### Structure
{% raw %}
```
{% assign object = object | sort: 'model' %}
{% for airliner in object %}
- [{{ airliner.company }} {{ airliner.model | capitalize }}]({{ airliner.model | prepend: '/airliner/' | url }})
{%- endfor %}
```
{% endraw %}