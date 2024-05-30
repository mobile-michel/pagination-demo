---
title: pagination variable
description: 
layout: default
tags: [primary, supplieddata]
date: 2024-03-11
pagination:
  data: object
  size: 1
---
{% include 'paginationObject' %}

- pagination.items[0] [objects]:
  {% for item in pagination.items[0] %}
  - pagination.items[0] {{ item | join: ": " }}
  {% endfor %}
- pagination.pageNumber: {{ pagination.pageNumber }}
- pagination.hrefs [array]: {{ pagination.hrefs | join: ", " }}
- pagination.href.previous: {{ pagination.href.previous | join: ", " }}
- pagination.href.next: {{ pagination.href.next | join: ", " }}
- pagination.href.first: {{ pagination.href.first | join: ", " }}
- pagination.href.last: {{ pagination.href.last | join: ", " }}
- pagination.pages[0] [objects]:
  {% for item in pagination.pages[0] %}
  - pagination.pages[0] {{ item | join: ": " }}
  {% endfor %}
- pagination.page.previous [objects]:
  {% for item in pagination.page.previous %}
  - pagination.page.previous {{ item | join: ": " }}
  {% endfor %}
- pagination.page.next [objects]:
  {% for item in pagination.page.next %}
  - pagination.page.next {{ item | join: ": " }}
  {% endfor %}
- pagination.page.first [objects]:
  {% for item in pagination.page.first %}
  - pagination.page.first {{ item | join: ": " }}
  {% endfor %}
- pagination.page.last [objects]:
  {% for item in pagination.page.last %}
  - pagination.page.last {{ item | join: ": " }}
  {% endfor %}
- pagination.data: {{ pagination.data }}
- pagination.size: {{ pagination.size }}
- pagination.alias: {{ pagination.alias }}