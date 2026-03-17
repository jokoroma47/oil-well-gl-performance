# Oil Well Performance Analytics — Gas Lift Optimisation & Production Intelligence

A data analytics project examining production behaviour 
across 13 gas lift wells, comparing three GL configurations 
and identifying pressure instability, fluid quality issues 
and operational anomalies across a 4-month monitoring period.

---

## Overview

Gas lift wells require continuous monitoring to maintain 
optimal production. Small changes in tubing head pressure, 
injection pressure or water cut can significantly affect 
lift efficiency and oil recovery. I built this project to 
analyse performance data across 13 wells, identify which 
configurations deliver the best results, and flag wells 
that require intervention.

The dataset covers 12,406 sub-daily readings across 13 
wells from June to October 2000, spanning three gas lift 
configurations — Short String, Long String and Standard GL.

---

## What I Found

- Well_286A has zero Casing Head Pressure for all 876 
  readings — gas injection is either inactive, a valve 
  is stuck closed, or the measurement system has failed. 
  This well requires immediate investigation
- Well_354 has a THP of 134 bar — 3.5x higher than any 
  other well in the field. This suggests a fundamentally 
  different reservoir pressure regime, possibly a naturally 
  flowing high-pressure well that does not require 
  conventional gas lift
- Long String GL wells show tubing annulus pressure 
  averaging 111 bar vs 30 bar for Standard GL — the TAP 
  difference is the clearest technical differentiator 
  between lift configurations in this field
- Five wells exceed 50% water cut — Wells 202, 295A, 206B, 
  209B and 284. High water cut significantly increases 
  lift energy requirements and reduces effective oil output
- Well_286A and Well_278 are the most pressure-unstable 
  wells, with THP coefficients of variation of 31.2% 
  and 24.3% respectively
- Well_296A appears in both Standard and Long String 
  datasets with identical readings — confirming it is a 
  deliberate A/B configuration comparison study
- Wells 206B and 209B share identical data across all 923 
  rows — these are likely the same physical well logged 
  under two IDs
- No H2S detected across any well or any reading — 
  field-wide safe conditions confirmed throughout

---

## Gas Lift Configurations

Three GL strategies are represented in this field. Standard 
GL uses mid-depth valve injection across 9 wells. Long 
String GL runs tubing to greater depth for deeper injection, 
used in Wells 284, 296A and 297A. Short String GL uses a 
shallower tubing string, represented by Well 278 alone.

---

## Dashboard

Five interactive pages covering — a field overview with 
all 13 wells ranked by THP and water cut, pressure analysis 
showing THP, CHP and TAP per well, fluid quality analysis 
across water cut and BS&W, GL configuration comparison 
showing how the three strategies differ in pressure 
behaviour, and a well health page with instability 
rankings and five detailed anomaly flags.

[View the live dashboard here](https://jokoroma47.github.io/oil-well-gl-performance)

---

## Tools Used

Power BI · MySQL · Python · HTML · CSS · JavaScript

---

## Files

| File | Description |
|------|-------------|
| index.html | Interactive web dashboard |
| data/oil_wells_cleaned.csv |

---
## Data Credit

Dataset: **Production dataset series**  
Source: Kaggle — [kaggle.com/datasets/sgobir/production-dataset/versions/1](https://www.kaggle.com/datasets/sgobir/production-dataset/versions/1)  
Author: sgobir  
Version: 1  

## Contact

**Portfolio:** [jokoroma47.github.io](https://jokoroma47.github.io)
**GitHub:** [@jokoroma47](https://github.com/jokoroma47)
**LinkedIn:** [linkedin.com/in/jeremiah-okoroma-724908116](https://linkedin.com/in/jeremiah-okoroma-724908116)
