# Donor Lifetime Value Prediction (UNICEF Case Study)

## Objective
Predict donor Lifetime Value (LTV) over the next 24 months using the first 90 days of donation behaviour, to support targeted fundraising and resource allocation.

## Context
University analytics project based on a real-world nonprofit fundraising scenario inspired by UNICEF Australia.

## Data
- ~1.78M transaction-level donation records
- Donor demographics, campaign attributes, and engagement indicators
- Data aggregated to donor level for modelling
(Data not shared publicly due to confidentiality.)

## Approach
- Data cleaning, transformation, and aggregation
- Exploratory Data Analysis (EDA)
- Feature engineering (RFM metrics, engagement indicators, target encoding)
- Two-stage **hurdle model**:
  - Classification: probability of future donation
  - Regression: donation magnitude conditional on giving
- Model comparison across linear and tree-based methods

## Models Used
- Logistic Regression (baseline)
- Random Forest
- Gradient Boosting
- XGBoost (final model)
- LightGBM
- CatBoost

## Results
- XGBoost achieved the strongest overall performance
- AUC ≈ 0.79 for donor reactivation
- RMSE ≈ $215 for LTV prediction
- Early donation frequency, recency, and monetary intensity were the strongest predictors

## Business Insights
- A small proportion of donors account for the majority of predicted value
- Early engagement behaviour is more predictive than demographics
- Supports targeted stewardship strategies for high-value donors

## My Contribution
- Led data cleaning, feature engineering, and EDA
- Implemented hurdle modelling framework
- Built and evaluated multiple ML models
- Interpreted results and translated findings into business recommendations

## Tools
Python, pandas, numpy, scikit-learn, XGBoost, LightGBM, CatBoost, matplotlib, seaborn, Jupyter Notebook
