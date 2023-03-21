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

### Geometry and ownership 
This inherits all of the rules of the inherited convention `farmOS:land:1.0`, with the following exceptions.

SHMU assets MUST include a polygon that represents their geographic boundaries in the "Intrinsic geometry" (`intrinsic geometry`) field.

SHMU asset MAY include at Type with the following labels:
- No Soil Health Practice Applied
- Soil Health Practice Applied

A single land owner or manager must be defined in a notes field.


### Land Use
SHMU asset MAY include a Type Narrative (free response string).

A single land use MUST be specified using one of the following labels:
- Crop
- Forest
- Range
- Pasture
- Farmstead
- Developed Land 
- Water
- Associated Agriculture Lands

One or more land use modifier MUST be specified using the following modifiers:
- None
- Drained
- Grazed
- Hayed
- Irrigated
- Organic
- Other
- Protected
- Water Feature
- Wildlife

One or more soil interpretations for MUST be specified in a free response text box. 

One or more soil drainage classes MUST be specified from the following list specified by SSURGO:
- Very Poorly Drained
- Poorly Drained
- Somewhat Poorly Drained
- Moderately Well Drained
- Well Drained
- Somewhat Excessively Drained
- Excessively Drained
- Saturated Muck
- Well Drained Muck
- Unknown

One or more hydrologic groups MUST be specified from the following list specified by NRCS National Engineering Handbook Part 630 Chapter 7 (https://directives.sc.egov.usda.gov/OpenNonWebContent.aspx?content=22526.wba):
- Group A
- Group B
- Group C
- Group D
- Group A/D
- Group B/D
- Group C/D

One or more ecological site ID  MUST be specified in a free response text box following the conventions defined in the National Ecological Site Handbook ([H_190_NESH_630-633)](https://www.nrcs.usda.gov/sites/default/files/2022-09/NESH_1.pdf)).

An Organic Matter indicator MUST be specified in ...

One or more site limitations actively being addressed MUST be selected from the following labels:
- None
- Poor Drainage
- Poor Organic matter
- etc (waiting to hear back on list)

One or more site limitations not being addressed MUST be selected from the following labels:
- None
- Poor Drainage
- Poor Organic matter
- etc (waiting to hear back on list)

One or more resource concern may be specified from the following labels, from the National Resource Concern List
and Planning Criteria:
- Air
- Animal
- Energy
- Human
- Plants
- Soil
- Water

One or more specific resource concerns MUST be specified from the following labels, from the National Resource Concern List
and Planning Criteria:
- none
- Aggregate Stability .. etc

Depending on specified land use, collect the following soil property data.

#### Land Use - Crop Land

One or more livestock grown on the land MAY be specified from the following labels:
- ..

One or more crop grown on the land MAY be specified from the following labels, and must be situated in a crop rotation. Should include cover crops from the following lables. Should be specified for all years of the agreement.
- crop list
- cover crop list (cover crop councils')

One or more inputs CAN be specified and MUST be assocated with an amount, frequency, and kind from the following lables.
- Fertilizer
- Pesticide
- Irrigation
- Ammendments
- ...

The current and previous tillage practices MAY be specified from the following labels, and must include number of years technique was included.:
- tbd



#### Land Use - Range Land

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
