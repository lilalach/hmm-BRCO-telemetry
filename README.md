# Hidden Markov Model for Animal Telemetry Data

This repository contains R code for fitting a 3-state hidden Markov model (HMM) to animal movement data using the `momentuHMM` package. The model incorporates GPS and dive data, and environmental covariates.

## Overview

The analysis is designed for reference and transparency, rather than full reproducibility. Input data files are not included in this repository due to size.

The main script file walks through:

1. **Loading libraries**
2. **Describing the preprocessing steps** that were done prior to this script
3. **Preparing cleaned data for HMM input**
4. **Exploring initial starting parameters** for model stability
5. **Fitting the HMM** using telemetry data and environmental covariates

## File Contents

- `hmm_workflow.R` — Main analysis script with full code, broken into clearly labeled steps.
- `output/` — Folder where you can save your fitted model object if desired.

## Requirements

- R version ≥ 4.0
- R packages:
  - `momentuHMM`
  - `tidyverse`
  - `lubridate`
  - `sf`
  - `plotly`
  - `tictoc`
  - `dplyr`

## Notes

- Input data is referenced as `"path/to/your/data_clean_formodels.rds"` and should include movement and environmental covariate data.
- Preprocessing steps (e.g., regularizing tracks, summarizing dives) are described in the comments but are not part of this script.
- This repository is meant to support the methods described in an accompanying manuscript.

