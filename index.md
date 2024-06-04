---
title: Home
description: These pages test arrays with different situations.
layout: default
tags: [primary, footer]
date: 2023-01-01
---
## Iteration tag
{% for item in collections.iteration %}
- [{{ item.data.title }}]({{ item.url | url }})
{%- endfor %}

## Pagination
{% for item in collections.pagination %}
- [{{ item.data.title }}]({{ item.url | url }})
{%- endfor %}

## Pagination with permalinks
{% for item in collections.permalink %}
- [{{ item.data.title }}]({{ item.url | url }})
{%- endfor %}

## Supplied data
{% for item in collections.supplieddata %}
- [{{ item.data.title }}]({{ item.url | url }})
{%- endfor %}