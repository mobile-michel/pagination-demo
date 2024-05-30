---
title: collections variable
description: 
layout: default
tags: [primary, supplieddata]
date: 2024-03-10
pagination:
  data: object
  size: 1
---
{% include 'paginationObject' %}

- collections.airliner[0].template [objects]:
  {% for item in collections.airliner[0].template %}
  - collections.airliner[0].template {{ item | join: ": " }}
  {% endfor %}
- collections.airliner[0].data [objects]:
  {% for item in collections.airliner[0].data %}
  - collections.airliner[0].data {{ item | join: ": " }}
  {% endfor %}
- collections.airliner[0].page [objects]:
  {% for item in collections.airliner[0].page %}
  - collections.airliner[0].page {{ item | join: ": " }}
  {% endfor %}
- collections.airliner[0].inputPath: {{ collections.airliner[0].inputPath }}
- collections.airliner[0].fileSlug: {{ collections.airliner[0].fileSlug }}
- collections.airliner[0].filePathStem: {{ collections.airliner[0].filePathStem }}
- collections.airliner[0].date: {{ collections.airliner[0].date }}
- collections.airliner[0].outputPath: {{ collections.airliner[0].outputPath }}
- collections.airliner[0].url: {{ collections.airliner[0].url }}
- collections.airliner[0].templateContent: {{ collections.airliner[0].templateContent }}
- collections.airliner[0].content: {{ collections.airliner[0].content }}