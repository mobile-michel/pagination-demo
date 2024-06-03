---
title: Important variables
description: 
date: 2024-09-10
pagination:
  data: object
  size: 4
---
### Page variables
- **title** : {{ title }}
- **page.fileSlug** : {{ page.fileSlug }}
- **page.filePathStem** : {{ page.filePathStem }}
- **page.url** : {{ page.url }}
- **page.inputPath** : {{ page.inputPath }}
- **page.outputPath** : {{ page.outputPath }}
- **page.date** : {{ page.date }}

### Collections variables
- **collections.airliner.size** : {{ collections.airliner.size }}
- **collections.airliner[0].data.title** : {{ collections.airliner[0].data.title }}
- **collections.airliner[0].fileSlug** : {{ collections.airliner[0].fileSlug }}
- **collections.airliner[0].filePathStem** : {{ collections.airliner[0].filePathStem }}
- **collections.airliner[0].url** : {{ collections.airliner[0].url }}
- **collections.airliner[0].inputPath** : {{ collections.airliner[0].inputPath }}
- **collections.airliner[0].outputPath** : {{ collections.airliner[0].outputPath }}
- **collections.airliner[0].date** : {{ collections.airliner[0].date }}
- **collections.airliner[0].templateContent** : {{ collections.airliner[0].templateContent }}

### Object variables from JSON file
- **object.size** : {{ object.size }}
- **object[0].model** : {{ object[0].model }}

### Pagination variables
- **pagination.size** : {{ pagination.size }}
- **pagination.pageNumber** : {{ pagination.pageNumber }}
- **pagination.items[0].model** : {{ pagination.items[0].model }}
- **pagination.href.next** : {{ pagination.href.next }}
- **pagination.href.last** : {{ pagination.href.last }}

### Eleventy filters
- **page.url | url** : {{ page.url | url }} (when pathPrefix is set)
- **title | slugify** : {{ title | slugify }}
- **"My Title" | log** : {{ "My Title" | log }}
- **assign previousPost = collections.airliner | getPreviousCollectionItem**
- **assign nextPost = collections.airliner | getNextCollectionItem**
- **assign index = collections.airliner | getCollectionItemIndex**
- **assign currentPost = collections.airliner | getCollectionItem**