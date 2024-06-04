---
title: eleventy variable
description: 
date: 2024-09-05
pagination:
  data: object
  size: 1
---
{% include 'pagination/object' %}

- **eleventy.version**: {{ eleventy.version }}
- **eleventy.generator**: {{ eleventy.generator }}
- **eleventy.env.source**: {{ eleventy.env.source }}
- **eleventy.env.runMode**: {{ eleventy.env.runMode }}
- **eleventy.env.config**: {{ eleventy.env.config }}
- **eleventy.env.root**: {{ eleventy.env.root }}
- **eleventy.env.isServerless**: {{ eleventy.env.isServerless }}