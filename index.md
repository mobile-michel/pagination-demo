---
title: Welcome to my test page
description: These pages test arrays with different situations.
layout: default
---
## Iteration tag
{% for item in collections.iteration %}
- [{{ item.data.title }}]({{ item.url }})
{%- endfor %}

## Pagination
{% for item in collections.pagination %}
- [{{ item.data.title }}]({{ item.url }})
{%- endfor %}

## Pagination with permalinks
{% for item in collections.permalink %}
- [{{ item.data.title }}]({{ item.url }})
{%- endfor %}

## Supplied data
{% for item in collections.supplieddata %}
- [{{ item.data.title }}]({{ item.url }})
{%- endfor %}