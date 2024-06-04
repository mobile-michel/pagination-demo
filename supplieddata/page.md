---
title: page variable
description: 
date: 2024-09-02
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