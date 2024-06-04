---
title: Paginate array
description: Uses the array.json data file to paginate over the array of airliners.
date: 2024-05-04
pagination:
  data: array
  size: 1
---
{% include 'pagination/array' %}

## {{ pagination.items | capitalize }}
### Structure
#### Frontmatter
```
pagination:
  data: array
  size: 1
```

#### Content
{% raw %}
```
{% include 'pagination/array' %}
## {{ pagination.items | capitalize }}
```
{% endraw %}

#### paginationArray
{% raw %}
```
<p>{% if page.url != pagination.href.first %}<a href="{{ pagination.href.first | url }}"><button>First page</button></a>{% else %}First page{% endif %} - 
{% if pagination.href.previous %}<a href="{{ pagination.href.previous | url }}"><button>{{ pagination.page.previous }}</button></a>{% else %}Previous{% endif %} - 
This is page {{ pagination.pageNumber | plus: 1 }} - 
{% if pagination.href.next %}<a href="{{ pagination.href.next | url }}"><button>{{ pagination.page.next }}</button></a> {% else %} Next{% endif %} - 
{% if page.url != pagination.href.last %}<a href="{{ pagination.href.last | url }}"><button>Last page</button></a>{% else %}Last page{% endif %}</p>
```
{% endraw %}