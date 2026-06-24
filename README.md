# Healthcare Diabetes Risk Analysis

## Project Overview

This project focuses on healthcare data cleaning and diabetes risk analysis using the CDC BRFSS 2015 survey dataset. The main objective is to prepare a clean and structured dataset for future exploratory data analysis and machine learning prediction.

## Dataset Source

The raw dataset comes from the CDC Behavioral Risk Factor Surveillance System (BRFSS) 2015.

Official source: https://www.cdc.gov/brfss/annual_data/annual_2015.html

The original dataset contains 441,456 records and 330 variables. In this project, selected healthcare, lifestyle, and demographic variables were extracted and cleaned.


## Data Cleaning Summary

The cleaning process was based on the official CDC BRFSS 2015 raw dataset and codebook. The objective was to prepare a clean and structured dataset for diabetes risk analysis while avoiding unnecessary data loss.

The cleaning process included:

- Selecting relevant healthcare, lifestyle, and demographic variables from the raw BRFSS dataset.
- Creating a binary diabetes target variable from `DIABETE3`.
- Removing unclear diabetes target responses to keep only confirmed diabetes and non-diabetes cases.
- Checking unclear and missing values before applying the final cleaning strategy.
- Handling missing and unclear values according to each variable type and missing-value percentage.
- Keeping unknown income responses as a separate category to avoid unnecessary data loss.
- Keeping unknown cholesterol-check and physical-activity responses as separate categories because of their relatively high missing or unclear rates.
- Converting BMI from `_BMI5` into readable BMI values and imputing missing BMI values using the median.
- Transforming alcohol consumption into estimated drinking days per month and imputing missing values using the median.
- Transforming fruit and vegetable consumption into estimated daily frequency and imputing missing values using the median.
- Removing old raw coded columns after creating clean replacement features.

## Final Cleaned Dataset

Final dataset shape:

```text
379,170 rows × 21 columns
