---
title: pkg variable
description: 
date: 2024-09-06
pagination:
  data: object
  size: 1
---
{% include 'pagination/object' %}

- **pkg.name**: {{ pkg.name }}
- **pkg.version**: {{ pkg.version }}
- **pkg.description**: {{ pkg.description }}
- **pkg.main**: {{ pkg.main }}
- **pkg.scripts** [objects]:
  {% for item in pkg.scripts %}
  - **pkg.scripts** [array] {{ item | join: ": " }}
  {% endfor %}
- **pkg.keywords** [array]: {{ pkg.keywords | join: ", " }}
- **pkg.author**: {{ pkg.author }}
- **pkg.license**: {{ pkg.license }}
- **pkg.devDependencies** [objects]:
  {% for item in pkg.devDependencies %}
  - **pkg.devDependencies**: {{ item }}
  {% endfor %}