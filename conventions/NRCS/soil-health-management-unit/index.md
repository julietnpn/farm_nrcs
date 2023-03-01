# Soil Health Management Unit

**Version 1.0**

```yml
convention_id: "NRCS:soil-health-management-unit:1.0"
dependencies:
inherits_from:
  - farmOS:land:1.0
  - nrcs:planning-land-unit:1.0
```

## Purpose

NRCS defines a SHMU as: 
```
Soil Health Management Unit (SHMU) is one or more planning land units with similar soil type, land use, and management that can vary in size or acreage depending on soil texture, topography, and cropping system. SHMU is like a conservation management unit but designed to assess soil health status and potential limitations on soil health indicators.
```

## Specification

This inherits all of the rules of the inherited convention nrcs:planning-land-unit:1.0, with the folowing exceptions.

Specifies similar qualities for one or more of the following categories regarding soil:
- interpretations for use
- drainage class
- hydrologic group
- ecological site
- soil health / organic matter

Specifies similar qualities in all of the management categories:
- crops and live stock grown
- kinds, amounts, and frequency of inputs
