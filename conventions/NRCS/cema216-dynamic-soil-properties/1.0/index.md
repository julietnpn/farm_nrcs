# CEMA 216 Dynamic Soil Properties

**Version 1.0**

```yml
convention_id: "NRCS:CEMA216-dynamic-soil-properties:1.0"
dependencies:
  - farm:farm_lab_test
inherits_from:
  - NRCS:CEMA216-Soil-Health-Test:1.0
  - farmOS:soil-test:1.0
related_conventions: NRCS:shmu:1.0
```

## Purpose

CEMA 216 Dynamic soil properties conduct the CEMA 216 Soil Health Test on two SHMUs with the same soil series for a comparative analysis to provide insight for planning purposes.

it to a soil testing lab, receiving test results back, and sending the data to the Soil Health Division for reporting. 

## Specification

This inherits all of the rules of the inherited convention NRCS:CEMA216-Soil-Health-Test:1.0, with the folowing exceptions.

Lab test logs MUST also reference specific SHMU assets in the "Location" (`location`) field to indicate where
the sample(s) were collected from for easier searching/filtering purposes. See related convention: NRCS:shmu:1.0



---

Questions for Mike:

1. We need to require the 216 soil health test twice, each on a different SHMU.
2. We need to require a log, which I think will be an observation.

## Specification for DSP Land Use Management Questionaire.