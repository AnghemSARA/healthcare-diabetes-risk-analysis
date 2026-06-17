# Healthcare Diabetes Risk Analysis

## Project Overview

This project focuses on healthcare data cleaning and diabetes risk analysis using the CDC BRFSS 2015 survey dataset. The main objective is to prepare a clean and structured dataset for future exploratory data analysis and machine learning prediction.

## Dataset Source

The raw dataset comes from the CDC Behavioral Risk Factor Surveillance System (BRFSS) 2015.

Official source: https://www.cdc.gov/brfss/annual_data/annual_2015.html

The original dataset contains 441,456 records and 330 variables. In this project, selected healthcare, lifestyle, and demographic variables were extracted and cleaned.

## Data Cleaning Summary

The cleaning process included:

- Selecting relevant healthcare variables from the raw BRFSS dataset.
- Creating a binary diabetes target variable.
- Removing unclear diabetes target responses.
- Handling missing and unclear values according to each variable type.
- Keeping unknown income responses as a separate category to avoid unnecessary data loss.
- Converting BMI from `_BMI5` into readable BMI values.
- Transforming alcohol consumption into estimated drinking days per month.
- Transforming fruit and vegetable consumption into estimated daily frequency.
- Removing old raw coded columns after creating clean replacement features.

## Final Cleaned Dataset

Final dataset shape:

```text
379,170 rows × 21 columns
