# Time Series Forecasting for Taxi Order Demand
## Project Overview
This project builds a time series forecasting model for Sweet Lift Taxi, a company operating airport taxi services. The core objective is to predict the number of taxi orders one hour into the future, helping the company optimize driver availability during peak times.

The model was evaluated using Root Mean Squared Error (RMSE) with a target performance threshold of less than 48 RMSE on the test set.

## Features & Functionality
Time Series Resampling: Converted raw 10-minute interval data into hourly time series.

Exploratory Data Analysis (EDA): Identified trends, daily seasonality, and data stationarity using Dickey-Fuller test and plots.

Feature Engineering:

Lag features

Rolling mean windows

Day of week indicators

Model Development:

Baseline Models: Median-based and rolling average models

Statistical Models: AR, ARIMA

Model Evaluation:

Metric: Root Mean Squared Error (RMSE)

Best model: Autoregressive (AR) with an RMSE of ~53.1

Tools Used:

pandas, matplotlib, statsmodels, scikit-learn

## Key Findings
Taxi demand increases during the week, particularly on Fridays and Mondays.

The time series exhibited stationary behavior despite visual non-stationarity, confirmed via the Dickey-Fuller test.

AR models outperformed other models, but the RMSE of 53.1 narrowly missed the target of 48.

## System Requirements
Python version: 3.9+

Recommended Libraries:

pandas>=1.3

numpy>=1.21

matplotlib>=3.4

scikit-learn>=1.0

statsmodels>=0.13

## Roadmap for Improvement
Fix prediction accuracy using cross-validation: Implement time series cross-validation (TimeSeriesSplit) to better assess overfitting and parameter tuning.

Fix RMSE gap using XGBoost or LSTM: Incorporate modern ML or deep learning models like XGBoost or LSTM to capture nonlinear patterns and improve performance.

Fix static feature handling using Fourier terms: Add Fourier series features for better modeling of weekly/daily seasonality trends.

Fix univariate limitation using weather/holiday data: Incorporate external features like weather, events, or holidays to improve model context awareness.

## Contributors
Project Author: Gabe Goodwin
