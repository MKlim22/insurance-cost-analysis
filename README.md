## Insurance Cost Analysis

## Overview
This project analyzes an insurance charges dataset and builds regression models to predict **charges**.

## Business Problem

Health insurance providers need to estimate medical costs based on customer characteristics such as age, BMI, smoking status, and family size.

The goal of this project is to analyze the factors that influence insurance charges and build regression models capable of predicting medical costs.
Understanding these relationships helps insurers better assess risk and design more accurate pricing models.

## Objectives
- Load the dataset into a pandas DataFrame
- Clean the data (handle missing/blank entries)
- Perform Exploratory Data Analysis (EDA)
- Build single-variable and multi-variable Linear Regression models
- Improve performance using Ridge Regression (regularization)

## Dataset
The lab uses a filtered/modified version of an insurance charges dataset (originally available on Kaggle).
To keep the repository clean and reproducible, the dataset file is not committed to Git.

Place the dataset here:
- `data/raw/insurance.csv`

## Methodology

The analysis follows a structured data science workflow:
1. Data loading and cleaning
2. Exploratory Data Analysis (EDA)
3. Baseline Linear Regression model
4. Interaction feature engineering (BMI x Smoking)
5. Residual analysis and model diagnostics
6. Model refinement using log transformation
7. Final model evaluation using R², MAE, and RMSE

## Project Structure

```
insurance-cost-analysis/
├─ README.md
├─ .gitignore
├─ requirements.txt
├─ data/
│ ├─ raw/
│ └─ processed/
├─ notebooks/
│ ├─ 01_import_clean.ipynb
│ ├─ 02_eda.ipynb
│ ├─ 03_modeling.ipynb
│ └─ 04_refinement.ipynb
├─ src/
└─ reports/
└─ figures/
```

## How to Run (local)
1. Create environment and install requirements
2. Run notebooks in order from `notebooks/`

## Results
The final interaction model (including BMI x Smoking) achieved:
- R² ~ 0.88
- Lower MAE and RMSE compared to alternative specifications

Smoking status was identified as the most influential factor affecting insurance cherges, with a strong interaction effect between BMI and smoking.

## Key Insights

- Smoking status is the strongest predictor of insurance charges
- BMI significantly increases medical costs among smokers
- Age has a steady positive effect on insurance costs
- Lifestyle-related factors play a major role in insurance pricing

The interaction model (BMI x Smoking) achieved the best performance with an R² of approximately 0.88.

## Future Improvements
- Compare additional models (e.g., RandomForestRegressor)
- Add proper train/validation/test workflow and cross-validation
- Package reusable functions in `src/`