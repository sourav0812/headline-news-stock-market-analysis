# Analyzing Headline News Impact on the Stock Market

## Overview
A Python-based data science project analyzing the relationship
between financial news sentiment and stock market performance
across major indices including NASDAQ, S&P500, AAPL, DJI, and NYA.

## Skills & Tools
- Python, Pandas, NumPy, Matplotlib, Seaborn
- NLP: VADER Sentiment Analysis (nltk), tokenization, lemmatization
- Linear Regression (OLS via statsmodels)
- Logistic Regression (Scikit-learn)
- VIF multicollinearity testing
- Time series analysis, IQR outlier detection, correlation matrices

## What This Project Does
1. Loads and preprocesses real stock market and headline data
2. Classifies market days as Bullish or Bearish based on NASDAQ trends
3. Runs VADER sentiment analysis on financial headlines to generate
   compound scores and categorizes them as positive, neutral, negative
4. Applies linear regression to assess whether sentiment scores
   predict AAPL stock prices (R² = 0.027 — statistically significant
   but weak predictor)
5. Applies logistic regression to predict Bullish vs Bearish market
   trend from sentiment scores
6. Performs advanced EDA including distribution analysis, correlation
   heatmaps, and time series plots highlighting the 2020 COVID crash
   and 2018-2019 Trade War period
7. Runs multiple regression with NASDAQ, NYA, SP500, DJI as
   predictors of AAPL prices (R² = 0.953) and tests for
   multicollinearity using VIF

## Key Findings
- Sentiment scores alone are weak predictors of stock prices
- Stock indices are highly correlated (AAPL-NASDAQ: 0.94)
- Multi-index regression achieves 95.3% explanatory power for
  AAPL prices
- High VIF scores confirm multicollinearity among indices

## Dataset
- stock_n_hl_news.csv — Daily stock prices and financial headlines
