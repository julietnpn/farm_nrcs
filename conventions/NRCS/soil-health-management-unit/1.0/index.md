# Soil Health Management Unit

**Version 1.0**

```yml
convention_id: "NRCS:soil-health-management-unit:1.0"
dependencies:
  - farm_nrcs:farm_nrcs_shmu
inherits_from:
  - farmOS:land:1.0
```

## Purpose

NRCS defines a SHMU as: 
```
Soil Health Management Unit (SHMU) is one or more planning land units with similar soil type, land use, and management that can vary in size or acreage depending on soil texture, topography, and cropping system. SHMU is like a conservation management unit but designed to assess soil health status and potential limitations on soil health indicators.
```
- SHMUs are created in CPA 116 dated 10/22/2022:
  - https://www.nrcs.usda.gov/sites/default/files/2022-10/FY23_CPA%20116_Soil%20Health%20Management%20Plan.pdf
- SHMUs are used in DIA 162 dated 10/22/2022:
  - https://www.nrcs.usda.gov/sites/default/files/2022-10/FY23_DIA%20162_Soil%20Health%20Management%20System%20Design.pdf
- SHMUs are used in CEMA 216 dated 10/22/2022:
  - https://www.nrcs.usda.gov/sites/default/files/2022-10/FY23_CEMA%20216_Soil%20Health%20Testing.pdf
- SHMUs are used in the Soil Health Demo Trials, dated 07/2022
  - https://cig.sc.egov.usda.gov/sites/default/files/2022-07/shdt_min_data_set_requirements_4722.pdf

## Specification

This inherits all of the rules of the inherited convention farmOS:land:1.0, with the following exceptions.

Land assets MUST include a polygon that represents their geographic boundaries in the "Intrinsic geometry" (intrinsic geometry) field.

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

Specifies similar qualities for one or more of the following categories regarding soil:
- interpretations for use
- drainage class
- hydrologic group
- ecological site
- soil health / organic matter

Specifies similar qualities in all of the management categories:
- crops and live stock grown
- kinds, amounts, and frequency of inputs


## Notable implementations

None.

## Changelog

#### 2023-03-01 - v1.0 (current version)

```yml
convention_id: "NRCS:soil-health-management-unit:1.0"
dependencies:
  - farm_nrcs:farm_nrcs_shmu
inherits_from:
  - farmOS:land:1.0
```

- First version.
