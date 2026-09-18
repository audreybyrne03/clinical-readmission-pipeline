# Clinical Readmission Prediction Pipeline

## Overview

The project uses the Diabetes 130-US Hospitals for Years 1999–2008 dataset
from the UCI Machine Learning Repository to explore the development of a
reproducible supervised classification pipeline for predicting early hospital
readmission among patients with diabetes.

## Dataset

**Dataset:** Diabetes 130-US Hospitals for Years 1999–2008  
**Source:** UCI Machine Learning Repository

The dataset contains 101,766 hospital encounters and 50 variables describing
demographics, hospitalization characteristics, diagnoses, laboratory testing,
medications, and prior healthcare utilization.

## Prediction Problem

The proposed classification task is to predict hospital readmission within
30 days of discharge.

The original `readmitted` variable contains three categories:

- `<30`: readmission within 30 days
- `>30`: readmission after 30 days
- `NO`: no recorded readmission

For the primary binary classification cohort:

- `1` = readmission within 30 days
- `0` = no recorded readmission

Encounters with readmission after 30 days are excluded from the primary
classification cohort.

## Current Analysis

The Week 3 exploratory analysis includes:

- Dataset import and structural assessment
- Definition of the binary classification target
- Descriptive statistics
- Assessment of missing data
- Exploratory visualization of candidate predictors
- Assessment of class imbalance
- Identification of preprocessing challenges
- Planning for subsequent supervised machine learning

## Repository Contents

- `Byrne_Engine.ipynb` — Jupyter notebook containing the analysis
- `diabetic_data.csv` — primary dataset
- `IDS_mapping.csv` — mappings for coded dataset variables
- `README.md` — project documentation

## Requirements

The notebook is designed for execution in Google Colab and uses:

- Python
- pandas
- NumPy
- Matplotlib

## Future Development

The final project will extend the exploratory workflow into a reproducible
classification pipeline including preprocessing, statistical analysis,
supervised machine-learning models, model evaluation, and interpretation.
