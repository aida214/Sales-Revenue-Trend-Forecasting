Sales/Revenue Trend Forecasting
Project Overview

This project analyses historical sales data and builds a time-series forecasting model to predict future sales. The goal is to help businesses make better decisions about inventory and staffing based on historical demand patterns.

Business Problem:

Businesses often plan inventory and staffing based on assumptions rather than actual historical sales patterns. This project uses historical sales data to identify trends and seasonal patterns and generate a forward-looking sales forecast.

Solution:

A time-series forecasting pipeline was developed using Python and Prophet. The project includes data cleaning, exploratory analysis, trend and seasonality analysis, model training, back testing, and a 90-day sales forecast with an uncertainty range.


Dataset:

The dataset contains daily sales data from:

1. January 2022 to December 2023
2. 730 unique dates
3. 10 stores

The dataset includes the following features:
1. Date
2. Store
3. Sales
4. Promotion
5. Holiday

Tools and Technologies:
1. Python
2. Pandas
3. Matplotlib
4. Prophet
5. Jupyter Notebook
6. Scikit-learn

Key Features:
1. Data cleaning and preprocessing
2. Daily sales trend analysis
3. 30-day moving average
4. Monthly sales analysis
5. Monthly seasonality analysis
6. Day-of-week sales analysis
7. Prophet forecasting model
8. Backtesting using held-out data
9. MAPE accuracy evaluation
10. 90-day sales forecast
11. Forecast uncertainty range


Model Evaluation:
The dataset was divided into training and testing data.

1. Training data: 640 days
2. Testing data: 90 days
3. Evaluation Metric: MAPE
4. Model MAPE: 1.88%

The backtesting results showed that the Prophet model was able to capture the main sales patterns and produce predictions close to the actual sales values.

Key Business Insights:
The analysis showed an overall increasing sales trend over time.
Sales also showed a strong weekly pattern. Sales were generally higher during the middle of the week and lower toward the weekend.
The 90-day forecast predicts continued sales patterns based on historical trends and weekly seasonality.
The uncertainty range provides a lower and upper estimate, helping businesses understand possible variations in future sales.

Challenges Faced:
1. Date Format Issue
The dataset contained dates in day/month/year format, which caused a date conversion error.
Solution: The date column was converted using the correct day-first format.

2. Prophet Installation
The Prophet library was initially not installed in the Python environment.
Solution: Prophet was installed and the Jupyter kernel was restarted.

3. Limited Historical Data
The dataset contained approximately two years of data, which could make yearly seasonality unstable.
Solution: Yearly seasonality was disabled, while weekly seasonality was retained based on the observed sales patterns.

Limitations:
1. Only two years of historical data were available.
2. External factors were not included in the forecasting model.
3. Promotions and holidays were not used as additional forecasting variables.
4. Unexpected events could affect future sales accuracy.


Future Improvements
Future versions of this project could include:
1. Promotion data as an additional forecasting feature
2. Holiday effects
3. Store-specific forecasting models
4. More historical data
5. Additional external factors
6. An interactive dashboard for business users


SafeX Relevance
This forecasting tool could be used as an internal business utility to help organizations predict future sales and demand. It could support better inventory planning, staffing decisions, and business forecasting.
The project could also be expanded into a future SaaS product with automated forecasting and interactive dashboards.


Aiyda Syed
Data Science
