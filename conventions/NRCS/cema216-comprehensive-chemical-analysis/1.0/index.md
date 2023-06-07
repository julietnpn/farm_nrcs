# CEMA 216 Comprehensive Chemical Analysis

**Version 1.0**

```yml
convention_id: "NRCS:CEMA216-comprehensive-chemical-analysis:1.0"
dependencies:
  - farm:farm_lab_test
inherits_from:
  - farmOS:soil-test:1.0
related_conventions: NRCS:shmu:1.0
```

## Purpose

CEMA 216 Comprehensive Chemical Analyses are used to provide information on soil nutrient content as it releates to healthy soil funciton and nutrient cycling.

These logs represent the act of collecting a soil sample, sending
it to a soil testing lab, receiving test results back, and sending the data to the Soil Health Division for reporting.

- Comprhensive Chemical Analyses are used in CEMA 216 dated 10/22/2022:
  - https://www.nrcs.usda.gov/sites/default/files/2022-10/FY23_CEMA%20216_Soil%20Health%20Testing.pdf

- Comprhensive Chemical Analyses are used in CEMA 217 dated 10/22/2022:?
  - 

## Specification

This inherits all of the rules of the inherited convention farmOS:soil-test:1.0, with the folowing exceptions.

The label MUST be one of the allowed labels listed below and adhere to the test method specified by the Modus Test ID of any Land Grant University that conducts this test method:
- phosphorus
  - Modus Test ID:
- potassium
  - Modus Test ID:
- calcium
  - Modus Test ID:
- magnesium
   - Modus Test ID:
- pH
  - Modus Test ID:
- sulfur
  - Modus Test ID:
- iron
  - Modus Test ID:
- manganese
  - Modus Test ID:  
- copper
  - Modus Test ID:  
- zinc
  - Modus Test ID:  
- boron
  - Modus Test ID:  
- cation exchange capacity
  - Modus Test ID:  
- total nitrogen
  - Modus Test ID:  

Lab test logs MUST also reference specific SHMU assets in the "Location" (`location`) field to indicate where
the sample(s) were collected from for easier searching/filtering purposes. See related convention: NRCS:shmu:1.0
