---
title: Collection tag
description: Uses the airliner tag in frontmatter to iterate over the airliners collection.
date: 2024-02-03
---
{% assign airliner = collections.airliner | sort: 'data.title' %}
{% for airliner in airliner %}
- [{{ airliner.data.title }}]({{ airliner.url | url }})
{%- endfor %}

### Structure
{% raw %}
```
{% assign airliner = collections.airliner | sort: 'data.title' %}
{% for airliner in airliner %}
- [{{ airliner.data.title }}]({{ airliner.url | url }})
{%- endfor %}
```
{% endraw %}