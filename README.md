# STRATOS: Garda Deployment Prediction — Python

**MSc Financial Technology — Programming for Financial Data Science**  
*National College of Ireland, Dublin | Student ID: 24198170*

---

## Overview

STRATOS is a Garda deployment prediction project built on officially published Irish crime incident data from 2003Q1 to 2025Q2. The goal is to quantify crime patterns across regions, offence types and time, then use machine learning to support data-informed Garda resource allocation decisions at quarter level.

The analysis is implemented in Python using a single end‑to‑end notebook, from raw CSV to engineered features, visual exploration and predictive modelling.

---

## Objectives

- Ingest and clean the original CSO crime incident dataset into a structured Pandas dataframe
- Engineer time-based features (Year, Quarter number) and structured region / offence codes
- Explore crime trends by Garda region, offence category and time using descriptive statistics and visualisations
- Standardise numeric features ready for modelling
- Train and evaluate tree-based regression models to predict incident counts (VALUE)
- Compare model performance and interpret which regions and offence types drive higher predicted Garda demand

---

## Data & Features

The notebook works with a crime incident dataset covering quarterly recorded offences with the following key fields:

- Quarter (e.g. 2003Q1, 2025Q2)
- Garda Region (Dublin Metropolitan, Eastern, North Western, Southern)
- Type of Offence and offence section codes
- VALUE: recorded crime incident counts
- Engineered features: Year, numeric quarter, region code, offence category and one‑hot encoded region indicators

The final modelling table contains VALUE as the target variable and a mix of temporal, regional and offence features as predictors.

---

## Methods

- Exploratory data analysis (EDA) using Pandas, Seaborn and Matplotlib
- Grouped aggregations and pivot-style summaries by region, offence and time
- Feature engineering for Year, Quarter number, Region and Offence
- Standardisation of numeric predictors using scikit-learn’s `StandardScaler`
- Supervised learning with:
  - DecisionTreeRegressor (limited depth)
  - RandomForestRegressor
- Train/test split evaluation and basic error metrics to compare models

---

## Tools & Technologies

| Tool | Purpose |
|------|---------|
| **Python 3** | Core programming language |
| **Pandas** | Data loading, cleaning, feature engineering |
| **NumPy** | Numerical operations |
| **Matplotlib / Seaborn** | Visualisation of crime trends and model insights |
| **scikit-learn** | Feature scaling and tree-based regression models |
| **Jupyter Notebook** | End-to-end analysis and modelling environment |

---

## How to Run

1. Clone this repository or download the files
2. Open the main `.ipynb` notebook in **Jupyter Notebook** or **Google Colab**
3. Ensure the crime CSV file is in the same folder as the notebook
4. Run all cells in order (Cell → Run All)

> **Requirements:** Python 3.x, pandas, numpy, matplotlib, seaborn, scikit-learn

---

## Author

**Mohd Nizam Nasir Shaikh**

MSc Financial Technology — National College of Ireland, Dublin

LinkedIn: https://www.linkedin.com/in/nizam-shaikh-90b737199  
GitHub: https://github.com/nizamshaikh12
