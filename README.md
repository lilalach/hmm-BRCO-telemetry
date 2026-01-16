# Hidden Markov Model for Brandt's Cormorant Telemetry Data

This repository contains R code specifically developed to fit a 3-state hidden Markov model (HMM) to telemetry data collected from Brandt's Cormorants in British Columbia, Canada. The analysis integrates GPS and dive data along with environmental covariates, as detailed in the accompanying manuscript. 

## Overview

This code supports the results and methods described in the manuscript by providing a transparent and reproducible workflow for fitting the HMM model to our cormorant telemetry data. It is not intended as a general-purpose HMM package or tutorial, but rather as a concrete example specific to this dataset and research questions.

## File Contents
- `hmm_workflow.R` — Script implementing the HMM fitting process step-by-step, including data preparation, parameter exploration, and model fitting.
- `output/` — Folder intended for saving model output objects.

## Data
Due to size and privacy, raw data files are not included here. The workflow assumes preprocessed telemetry and environmental covariate data in the form of "path/to/your/data_clean_formodels.rds". Preprocessing steps are described in the manuscript and in the comments of the script.

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

The code is tailored to our specific dataset and analysis goals. Adapting it to other species or data may require modification. It has not been generalized, optimized, or tested for use with other datasets.

Comments within the script describe preprocessing assumptions and model fitting details.
This repository is meant to support the methods described in an accompanying manuscript.

