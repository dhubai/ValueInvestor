# SmartInvestor: Intelligent Stock Investment System

## Overview

**SmartInvestor** is an intelligent stock investment system developed for a portfolio investment company focusing on emerging markets. The system aids in making data-driven investment decisions by predicting stock price valuations on a daily, weekly, and monthly basis. The primary goal is to maximize capital returns, minimize losses, and optimize the hold period for stocks.

## Project Objective

The project aims to create a robust machine learning-based system that recommends BUY, HOLD, or SELL decisions based on historical stock price data. The system evaluates performance using Bollinger Bands, LSTM neural networks, and Facebook Prophet to assess capital returns and minimize holding periods. 

## Data Description

The dataset consists of trading data from emerging market portfolio companies, including 2020 quarterly data (Q1-Q4) and 2021 Q1 data. The stock prices for each company are provided in different sheets, with varying market operating days based on the country and exchange.

- **Data Utilized:** Only 2020 data is used for training, and 2021 Q1 data is used for prediction.

## Methodology

### 1. Data Preparation
- Cleaned and preprocessed data to remove outliers, duplicates, and missing values.
- Converted stock prices to numerical format and dates to datetime format for consistency.

### 2. Feature Engineering
- Calculated 20-day Exponential Moving Average (EMA) and Bollinger Bands to identify potential buy/sell signals.
- Generated trading signals based on Bollinger Bands for buy, sell, or hold recommendations.

### 3. Forecasting Models
- **Facebook Prophet**: Used for time series forecasting to predict future stock prices. 
  - *Mean Absolute Percentage Error (MAPE):* 
    - Egypt, Medinet Nasr Housing (MNHD): 21.11%
    - Colombia, Cementos Argos SA (CCB): 25.63%
- **LSTM Neural Network**: Used for sequential stock price predictions.
  - *MAPE Results:*
    - Egypt, Medinet Nasr Housing (MNHD): 1.68%
    - Colombia, Cementos Argos SA (CCB): 2.08%

### 4. Trading Simulation
- Simulated trading with an initial capital of $10,000 to evaluate the system's performance.
- Calculated total capital returns based on the generated signals:
  - Egypt, Medinet Nasr Housing (MNHD): 2.41%
  - Colombia, Cementos Argos SA (CCB): 133.36%

## Key Results

- **Prophet Forecasting Performance:**
  - Achieved MAPE of 21.11% for Medinet Nasr Housing and 25.63% for Cementos Argos.
- **LSTM Model Performance:**
  - Achieved MAPE of 1.68% for Medinet Nasr Housing and 2.08% for Cementos Argos.
- **Trading Simulation:**
  - Total capital returns of 2.41% for Medinet Nasr Housing and 133.36% for Cementos Argos.

## Conclusion

The SmartInvestor system effectively uses machine learning models to predict stock price movements and optimize investment decisions. The LSTM model outperformed Facebook Prophet in terms of accuracy, and the trading strategy resulted in substantial returns for selected stocks.


