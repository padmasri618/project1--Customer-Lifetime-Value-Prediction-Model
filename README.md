## Objective
- To accurately predict Customer Lifetime Value using historical customer data, including demographics and behavioral patterns. The goal is to help businesses:

- Improve marketing ROI through customer segmentation.

- Focus on high-value customers.

- Drive personalized strategies for retention and growth.
---
## Dataset
- File Used: Customer_Lifetime_Value_Prediction.csv

- Key Features:

- Demographics: Age, Gender, Tenure

- Behavioral: NumPurchases, TotalSpend, AvgPurchaseValue, RecencyDays, FrequencyPerMonth

- Target: LifetimeValue (continuous)
- -
## Tools & Technologies
- Python: pandas, numpy, matplotlib, seaborn, scikit-learn

- Excel: Dashboard with visual insights

- Machine Learning: Random Forest Regressor (main model)

-- 
## Methodology
- Data Cleaning:

- Handled missing values and outliers.

- Converted data types appropriately.

- Removed duplicates.

- Feature Engineering:

- Derived Recency, Frequency, and Avg Purchase Value.

- Standardized numeric values.

- One-hot encoded categorical features.

- Model Building:

- Used RandomForestRegressor and optionally XGBoost.

- Evaluated with MAE and RMSE.

- Random Forest was chosen for final predictions.

- Segmentation:

- Used pd.qcut() to divide predicted CLTV into 3 segments: Low, Medium, High.

- Visualization:

- EDA plots, heatmaps, boxplots.

- Excel dashboard: Pie, Line, and Bar charts.

--
## Results
- Model Metrics:

- MAE ≈ 338.79

- RMSE ≈ 457.30

- Customer Segments:

- Low: 334 customers | Avg LTV ≈ 1897.75

- Medium: 333 customers | Avg LTV ≈ 3478.33

- High: 333 customers | Avg LTV ≈ 5358.38

--
## Key Insights
- Most customers fall in the Low-Medium range—potential to upsell.

- High LTV customers are fewer but generate significant revenue.

- Recency-Frequency relationship can signal churn risks or loyal behavior.

- Medium-value customers can be nurtured to become high-value.

--
## Deliverables
-  Python Notebook (CLTV.ipynb)

-  Final Predictions CSV (final_ltv_predictions.csv)

 - Excel Report with Charts

-  PDF Summary Report (LTV_Prediction_Report.pdf)

- Documentation (CLTV.odt)
