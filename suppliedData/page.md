---
title: page variable
description: 
layout: default
tags: [primary, supplieddata]
date: 2024-09-12
pagination:
  data: object
  size: 1
---
{% include 'pagination/object' %}

- **page.url**: {{ page.url }}
- **page.outputPath**: {{ page.outputPath }}
- **page.date**: {{ page.date }}
- **page.inputPath**: {{ page.inputPath }}
- **page.fileSlug**: {{ page.fileSlug }}
- **page.filePathStem**: {{ page.filePathStem }}
- **page.outputFileExtension**: {{ page.outputFileExtension }}
- **page.templateSyntax**: {{ page.templateSyntax }}