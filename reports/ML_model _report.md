# House Price Prediction with Machine Learning

## Overview

This repository contains a machine learning notebook for predicting house prices based on a synthesized real estate dataset with 70,000 entries. The analysis includes data exploration, feature engineering, and regression modeling using Decision Tree and XGBoost regressors with detailed evaluation metrics.

---

## Dataset Description

The dataset contains 70,000 entries with 23 features, including numerical, categorical, and boolean types. Key features include:

- `location`: City and state (e.g., San Diego, CA)
- `region_type`: Urban or Suburban
- `property_type`: Property category (e.g., House, Loft)
- `year_built`
- `condition`, `furnishing` (categorical)
- `bedrooms`, `bathrooms` (parsed numerically)
- `stories`, `parking`, `garden` (boolean)
- `lot_area_sqft`, `floor_area_sqft`
- Financial features such as `property_tax_usd`, `insurance_usd`, `maintenance_usd`, `rent_usd_month`
- Demographic and safety indices like `median_income_usd`, `employment_rate`, `crime_index`, `safety_index`

New features such as `property_age` and a composite `living_level_score` were also created.

---

## Exploratory Data Analysis

- Visualized distribution of house prices overall and by categories (location, property type, furnishing, region type).
- Correlation heatmaps revealed relationships between numerical variables.
- Boxplots identified outliers and spread in financial and size-related features.
- Displayed detailed data for the top 10 highest priced properties.

---

## Feature Engineering

- Converted categorical variables with label encoding or one-hot encoding.
- Extracted numeric bathroom counts from text fields.
- Scaled numerical features with `StandardScaler`.
- Created composite scores to capture living environment quality.

---

## Modeling Approach

Two separate models were trained and evaluated:

- **Decision Tree Regressor**
- **XGBoost Regressor**

Both models were trained on 80% of the data and tested on the remaining 20%. Additionally, 5-fold cross-validation was used to estimate generalization error via RMSE.

Evaluation metrics reported include:

- Mean Squared Error (MSE)
- Root Mean Squared Error (RMSE)
- Mean Absolute Error (MAE)
- R-squared (R2)

---

## Results Summary

| Model            | CV Mean RMSE | Train RMSE | Test RMSE | Train R2 | Test R2 |
|------------------|--------------|------------|-----------|----------|---------|
| Decision Tree    | 2292.87      | 2261.51    | 2240.37   | 0.9994   | 0.9994  |
| XGBoost          | 2109.09      | 1130.98    | 1836.44   | 0.9999   | 0.9996  |

XGBoost outperformed the decision tree with lower error and better generalization.

---

## How to Run

1. Clone the repository.
2. Install dependencies (e.g., via `pip install -r requirements.txt`).
3. Download or place the dataset `real_estate_agent.csv` in the appropriate directory and update the file path in the notebook if needed.
4. Run the notebook cells sequentially to reproduce data processing, modeling, and evaluation.

---

## Dependencies

- Python 3.8+
- numpy
- pandas
- scikit-learn
- matplotlib
- seaborn
- xgboost

---

## License

The dataset is synthetic, and no license is required for this project.
