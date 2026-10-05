---
date: '2026-06-10' 
title: 'Hydrological Modelling of the Kammel Catchment'
github: 'https://github.com/HumzAhme/Hydrological-Modelling-Kammel-Catchment'
external: ''
tech:
  - R 
  - airGR
  - HBV.IANIGLA
  - Python
  - Quarto
  - Git
company: 'Leipzig Uni'
showInProjects: true
---

- Built daily catchment-average precipitation and temperature from gridded DWD data (HYRAS) and computed evapotranspiration with the Hargreaves-Samani method.
- Calibrated GR4J (no snow module), HBV and GR6J (airGR Calibration_Michel, SCE-UA) using a swapped split-sample design (1988–1999 / 2000–2010), then simulated daily streamflow for 2011–2020, a decade with no gauge data.
- Quantified four uncertainty sources separately: model parameters (top 1% parameter sets), model structure, calibration period, and input data (HYRAS vs. a second precipitation/temperature product, EDK).
- Ran a counterfactual climate-change experiment: removed an estimated warming and drying trend from the forcing and compared summer (June–August) discharge with and without it.

- GR6J, with its extra slow groundwater store, scored best on NSE (about 0.70–0.73 in validation), matching the catchment's high baseflow index (0.74). The ranking changed under KGE, so the "best" model depended on the metric.
- Parameter and structural uncertainty were largest; the input dataset mattered least (mean streamflow difference 0.07 mm/day).
- Snow parameters were poorly identified because the catchment sees little snow (about 15% of days below freezing). HBV was most sensitive to calibration period.
- Climate change is estimated to have already reduced mean summer discharge by roughly 15%, using literature-based trend values.

- GR4J modelling, aligning GR4J's calibration setup with GR6J's so the models could be compared fairly, and the counterfactual analysis.

