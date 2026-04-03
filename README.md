# ARIMA-Momentum-Threshold-Strategy
## What is ARIMA?

ARIMA stands for **AutoRegressive Integrated Moving Average**. It is a time-series model used to describe and forecast data based on its past behavior.

It consists of three components:

- **AR (AutoRegressive):** captures persistence (momentum)
- **I (Integrated):** removes trend via differencing
- **MA (Moving Average):** captures the effect of past shocks (errors)

In this notebook, we use ARIMA(1,1,1):
- 1 lag of past changes (AR)
- 1 differencing step
- 1 lag of past errors (MA)

## Why use ARIMA?

We want to test whether past BTC price movements contain information that can help predict future prices.

If the model predicts:
- a higher price → go long
- a lower price → go short

This allows us to turn a statistical model into a trading strategy.

## Key Takeaways

- ARIMA can capture structure in time series data
- However, short-term crypto markets are very noisy
- Simple models often fail after transaction costs
- This is a useful framework, but not a complete trading system
