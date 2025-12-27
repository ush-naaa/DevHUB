# Energy Consumption Time Series Forecasting

## Objective
The objective of this project is to forecast short-term household energy consumption
using historical time series data. By applying time-series feature engineering and
comparing multiple forecasting models, the goal is to identify the most effective
approach for predicting future energy demand to support efficient energy management
and planning.

---

## Dataset
**Household Power Consumption Dataset**

The dataset contains household electricity usage records collected over time,
including the following attributes:
- Date and Time
- Global Active Power
- Global Reactive Power
- Voltage
- Global Intensity
- Sub-metering 1, 2, and 3

The dataset was sourced from Kaggle and resampled to an hourly frequency for analysis.

---

## Approach
The following steps were followed in this project:

1. Loaded and explored the time-series dataset
2. Parsed date and time fields and handled missing values
3. Resampled the data to an hourly frequency to reduce noise
4. Engineered time-based features such as hour of day and day of week
5. Created lag features representing previous hour and previous day consumption
6. Trained and compared multiple forecasting models including ARIMA, Prophet,
   and XGBoost
7. Evaluated model performance using RMSE and visualized actual vs. forecasted values

---

## Results & Insights
The comparison of forecasting models showed noticeable differences in performance.
Traditional time-series models captured general trends, while machine learning models
benefited from engineered lag features.

The XGBoost model achieved the lowest RMSE, indicating superior predictive accuracy
for short-term energy consumption forecasting.

---

## Model Performance (RMSE)
- **ARIMA:** 0.75
- **Prophet:** 0.62
- **XGBoost:** 0.50 (Best Performance)

---

## Conclusion
This project demonstrates the importance of feature engineering in time-series
forecasting. While ARIMA and Prophet effectively modeled seasonal patterns, XGBoost
outperformed them by leveraging lag-based features that capture short-term dependency
in energy consumption data. These results highlight the value of machine learning
approaches for accurate energy demand forecasting.
