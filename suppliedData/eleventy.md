---
title: eleventy variable
description: 
layout: default
tags: [primary, supplieddata]
date: 2024-03-13
pagination:
  data: object
  size: 1
---
{% include 'paginationObject' %}

- **eleventy.version**: {{ eleventy.version }}
- **eleventy.generator**: {{ eleventy.generator }}
- **eleventy.env.source**: {{ eleventy.env.source }}
- **eleventy.env.runMode**: {{ eleventy.env.runMode }}
- **eleventy.env.config**: {{ eleventy.env.config }}
- **eleventy.env.root**: {{ eleventy.env.root }}
- **eleventy.env.isServerless**: {{ eleventy.env.isServerless }}