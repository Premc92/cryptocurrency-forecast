# Cryptocurrency Time-Series Forecasting

## Project overview
An educational time-series forecasting project using historical cryptocurrency market data. It demonstrates time-indexed data preparation, forecasting and evaluation. Forecasts are uncertain and should not be interpreted as investment advice.

## Business and analytical questions
- How do price and volume behave over the selected historical window?
- How does a forecasting model compare with a simple naive baseline?
- How does forecast error change across the evaluation period?
- Are results robust to a time-ordered holdout rather than a random split?

## Existing notebook
- `Cryptocurrecny.ipynb` — original cryptocurrency forecasting analysis.

## Improvement plan
1. Make the ticker, frequency, start date and end date configurable.
2. Validate missing dates, duplicate timestamps and missing market observations.
3. Use a chronological train/validation/test design; never shuffle time-series observations.
4. Compare the selected model with naive and seasonal-naive baselines.
5. Report MAE and RMSE; use MAPE only when its denominator is meaningful and non-zero.
6. Plot actuals, forecasts and residuals with a clearly labelled forecast horizon.
7. Record data-source limitations, market regime changes and the risk of overfitting.

## Tools
Python, pandas, NumPy, yfinance and forecasting libraries used in the notebook.

## Responsible interpretation
Historical patterns do not guarantee future returns. Cryptocurrency markets are volatile, non-stationary and affected by events that a historical model may not capture. This project is for technical learning only, not trading recommendations.
