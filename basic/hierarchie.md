---
title: Hierarchical JSON
description: Uses the hierarchic.json data file to iterate over the airliner's objects & arrays.
date: 2024-02-03
---
{% for role_names in hierarchic %}
{%- for company_names in role_names.airplanes %}
{%- for airplanes_names in company_names.models %}
- [{{ company_names.company }} {{ airplanes_names.model | capitalize }}]({{ airplanes_names.model | prepend: '/airliner/' | url }})
{%- endfor %}
{%- endfor %}
{%- endfor %}

### Structure
{% raw %}
```
{% for role_names in hierarchic %}
{%- for company_names in role_names.airplanes %}
{%- for airplanes_names in company_names.models %}
- [{{ company_names.company }} {{ airplanes_names.model | capitalize }}]({{ airplanes_names.model | prepend: '/airliner/' | url }})
{%- endfor %}
{%- endfor %}
{%- endfor %}
```
{% endraw %}