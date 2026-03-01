# Silondile-mavundla-
# JSE Volatility Analysis

A comprehensive financial analysis project examining the volatility patterns of Naspers (NPN.JO) listed on the Johannesburg Stock Exchange (JSE).

## Overview

This project analyzes historical stock price data from 2015 to 2024 to understand volatility patterns, return distributions, and market behavior. Using advanced statistical methods and time-series analysis, we explore whether stock returns are predictable and how risk fluctuates over time.

## Objectives

- Analyze daily log returns of Naspers stock
- Test for stationarity in return series
- Investigate predictability of stock returns
- Identify volatility clustering patterns
- Visualize risk evolution over time

## Features

- **Data Retrieval**: Automated download of historical stock data using yfinance
- **Statistical Testing**: Augmented Dickey-Fuller (ADF) test for stationarity
- **Regression Analysis**: OLS regression to test return predictability
- **Volatility Analysis**: 30-day rolling volatility calculations
- **Visualizations**: Time-series plots for returns and volatility

## Dataset

- **Ticker**: NPN.JO (Naspers Limited)
- **Period**: January 1, 2015 - December 31, 2024
- **Frequency**: Daily closing prices
- **Observations**: 2,525 trading days

## Key Findings

### Returns Analysis
- **Mean Daily Return**: 0.0583% (≈0.583 basis points)
- **Standard Deviation**: 2.42%
- **Range**: -19.48% to +20.53%
- **Conclusion**: Little evidence of predictable returns (median return near zero)

### Stationarity Test
- **ADF Statistic**: -17.90
- **P-value**: 2.96e-30 (highly significant)
- **Conclusion**: Returns are strongly stationary

### Predictability Test
- **R-squared**: 0.000 (no explanatory power)
- **Lag Return Coefficient**: -0.0135 (p-value: 0.497)
- **Conclusion**: Previous returns do not significantly predict future returns

### Volatility Patterns
- **Observation**: Clear evidence of volatility clustering
- **Pattern**: Risk fluctuates significantly over time with identifiable periods of high and low volatility
- **Implication**: Future volatility partly depends on historical volatility

## Installation

### Prerequisites
- Python 3.8+
- Jupyter Notebook or Google Colab

### Required Libraries

```bash
pip install yfinance statsmodels pandas numpy matplotlib
