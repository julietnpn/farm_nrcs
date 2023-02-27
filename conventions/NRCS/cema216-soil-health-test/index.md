# CEMA 216 Soil Health Indicator Test

**Version 1.0**

```yml
convention_id: "NRCS:CEMA216-soil-health-test:1.0"
dependencies:
  - farm:farm_lab_test
inherits_from:
  - farmOS:soil-test:1.0
related_conventions: NRCS:shmu:1.0
```

## Purpose

CEMA 216 Soil Health Tests are used to represent the act of collecting a soil sample, sending
it to a soil testing lab, receiving test results back, and sending the data to the Soil Health Division for reporting. 

## Specification

This inherits all of the rules of the inherited convention farmOS:soil-test:1.0, with the folowing exceptions.

The label should be one of the allowed labels listed below, or it should be the csv column header from the lab:
- Soil Organic Carbon
- Wet Macro-Aggregate Stability
- Respiration
- Active Carbon
- Bioavailable Nitrogen using ACE Protien
- Microbial Diversity using PFLA

Lab test logs MUST also reference specific SHMU assets in the "Location" (`location`) field to indicate where
the sample(s) were collected from for easier searching/filtering purposes. See related convention: NRCS:shmu:1.0
