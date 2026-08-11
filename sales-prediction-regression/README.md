# Sales Prediction using Multiple Linear Regression

Built a multiple linear regression model to predict product sales based on advertising expenditure across TV, radio, and newspaper channels.

## Dataset
200 records of advertising spend (TV, Radio, Newspaper) and resulting Sales.

## Approach
- Cleaned the data (handled missing values)
- Explored correlations between each advertising channel and sales
- Trained a multiple linear regression model (80/20 train-test split)
- Evaluated performance using R², RMSE, and MAE
- Compared model performance on raw vs. normalized data
- Tested a reduced feature subset (dropping TV) to measure its impact on accuracy

## Key Findings
- TV spend had the strongest correlation with sales (r ≈ 0.90), far more than radio (r ≈ 0.35) or newspaper (r ≈ 0.16)
- The full model achieved a test R² of ≈ 0.90
- Normalization had no effect on performance, as expected for linear regression (it's scale-invariant)
- Dropping TV from the feature set caused the model's test R² to collapse (from ≈ 0.90 to slightly negative), confirming TV is the dominant driver of sales in this dataset

## Tools
Python, Pandas, Scikit-learn, Matplotlib
