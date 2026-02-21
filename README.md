# Insurance Cost Analysis

## Overview
This project analyzes an insurance charges dataset and builds regression models to predict **charges**.

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
(To be added)

## Future Improvements
- Compare additional models (e.g., RandomForestRegressor)
- Add proper train/validation/test workflow and cross-validation
- Package reusable functions in `src/`