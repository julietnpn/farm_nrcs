# Planning Land Unit

**Version 1.0**

```yml
convention_id: "NRCS:planning-land-unit:1.0"
dependencies:
inherits_from:
  - farmOS:land:1.0
```

## Purpose

Planning Land Units (PLU) are a core map unit used by USDA NRCS in conservaiton planning. NRCS defines a PLU as: 
```
A PLU is a unique geographic area, defined by a polygon, that has common land use and is owned, operated, or managed by the same client or clients. The PLU is the minimum unit for planning.
```
**Link a reference**

## Specification

This inherits all of the rules of the inherited convention farmOS:land:1.0, with the folowing exceptions.

The polygon must be defined.

A common land use must be specified using one of the following labels:
- Crop
- Forest
- Range
- Pasture
- Farmstead
- Developed Land 
- Water
- Associated Agriculture Lands

A single land owner or manager must be defined in a notes field.
