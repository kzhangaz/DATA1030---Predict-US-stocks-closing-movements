# Predict US Stocks Closing Movements

## Introduction

This repository contains a machine learning project undertaken as part of the DATA 1030 Hands-on Data Science course at Brown University. The project focuses on predicting the closing price movements of numerous Nasdaq-listed stocks using historical data from the daily ten-minute closing auction.

## Project Goal

The primary objective is to develop machine learning models for regression to predict future stock price movements. The project utilizes historical data provided by Optiver on KaggleOptiver (2023), specifically from the daily ten-minute closing auction. This period is crucial for decision-making and influences market sentiment, making it an opportune time for making informed predictions about stock prices.


## Dataset Description

### Overview

The dataset contains historic data from the daily ten-minute closing auction on the NASDAQ stock exchange. It presents a unique challenge of predicting future price movements for individual stocks relative to a synthetic index composed of NASDAQ-listed stocks. You can visit it on Kaggle at [here](https://www.kaggle.com/competitions/optiver-trading-at-the-close).

### Key Features

1. **Imbalance Buy/Sell Flag:** An indicator reflecting the direction of auction imbalance: 1 for Buy-side imbalance, -1 for Sell-side imbalance, and 0 for No imbalance.
2. **Bid/Ask Price:** Represents the price of the most competitive buy/sell level in the non-auction book.
3. **Bid/Ask Size:** Indicates the dollar notional amount on the most competitive buy/sell level in the non-auction book.
4. **WAP (Weighted Average Price):** The weighted average price in the non-auction book.
5. **Target:** Represents the 60-second future move in the WAP of the stock, less the 60-second future move of the synthetic index. The unit of the target is basis points, equivalent to a 0.01% price move.

### Dataset Details

The dataset includes information on 200 distinct stocks, meticulously documented across more than 20,000 data points. These data points capture the nuances of each stock during the daily closing auction period, forming a time series with a discernible group structure that encapsulates the dynamic evolution of each stock over time.

## Models

Our forecasting machine learning pipeline encompasses
four distinct models: Linear Regression, XGBoost, Random Forest, and K Nearest Neigh-
bors.
