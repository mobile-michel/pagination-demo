---
title: JSON files
description: structure of JSON files.
layout: default
tags: [primary, supplieddata]
date: 2024-12-01
---
### array.json
- (array)
  - (names of airliners)

### object.json
- (array of objects)
  - model
  - role
  - service
  - description

### hierarchic.json
- (array of objects)
- role
- role_description
- airplanes (array of objects)
  - company
  - models (array of objects)
    - model
    - service
    - description