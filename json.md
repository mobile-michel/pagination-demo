---
title: JSON files
description: Structure of JSON files.
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
  

### array.json file
```
[
    "a220",
    "a320",
    "a380",
    "b717",
    "b737",
    "b787",
    "a350",
    "b777"
]
```

### object.json file
```
[
    {
        "company": "Airbus",
        "model": "a220",
        "role": "Narrow-body jet airliner",
        "role_description": "A narrow-body aircraft or single-aisle aircraft is an airliner arranged along a single aisle permitting up to 6-abreast seating in a cabin below 4 metres (13 ft) of width.",
        "service": "2012",
        "description": "The Airbus A220 is a family of five-abreast narrow-body airliners by Airbus Canada Limited Partnership (ACLP). It was originally developed by Bombardier and had two years in service as the Bombardier CSeries."
    }
]
```
### collections.airliner tag
```
---
title: Airbus 220
role: Narrow-body jet airliner
service: 2012
---
The Airbus A220 is a family of five-abreast narrow-body airliners by Airbus Canada Limited Partnership (ACLP). It was originally developed by Bombardier and had two years in service as the Bombardier CSeries.
```

### hierarchic.json file
```
[
    {
        "role": "Narrow-body jet airliner",
        "role_description": "a narrow-body aircraft or single-aisle aircraft is an airliner arranged along a single aisle, permitting up to 6-abreast seating in a cabin below 4 metres of width.",
        "airplanes": [
            {
                "company": "Airbus",
                "models": [
                    {
                        "model": "a220",
                        "service": "2012",
                        "description": "the Airbus A220 is a family of five-abreast narrow-body airliners by Airbus Canada Limited Partnership (ACLP). It was originally developed by Bombardier and had two years in service as the Bombardier CSeries."
                    }
                ]
            }
        ]
    }
]
```