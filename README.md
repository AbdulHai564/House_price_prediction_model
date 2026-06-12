# House Price Prediction 

## Overview
Built a machine learning model to predict house sale prices using regression techniques and feature engineering.

## Dataset
1460 houses with 79 features from Ames, Iowa

Download from Kaggle:
 https://www.kaggle.com/competitions/house-prices-advanced-regression-techniques/data

## What I did
- Handled missing values (dropped >40% missing, filled rest with median/mode)
- Feature engineering — created 6 new meaningful features
- Encoded 43 categorical columns using LabelEncoder
- Trained Linear Regression and Random Forest Regressor
- Compared models using R2, MAE and RMSE

## Feature Engineering
- TotalSF = 1st floor + 2nd floor area
- HouseAge = Year sold - Year built
- YearsSinceRemodel = Year sold - Year remodeled
- HasGarage, HasPool, HasBasement (binary flags)

## Libraries
pandas, numpy, sklearn, plotly, matplotlib

## Results
| Model | R2 | MAE | RMSE |
|---|---|---|---|
| Linear Regression | 85.4% | $20,609 | $33,357 |
| Random Forest | 89.3% | $17,616 | $28,553 |

## Key Findings
- Random Forest outperforms Linear Regression on all metrics
- Overall quality and total square footage are top price predictors
- Feature engineering improved R2 from 88.5% to 89.3%

## How to Run
1. Download dataset from Kaggle link above
2. Install requirements: pip install pandas numpy sklearn matplotlib plotly
3. Open notebook in Jupyter or VS Code
4. Run all cells in order
