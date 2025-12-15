# bitcoin-price-analysis
Exploratory data analysis of Bitcoin price, volatility, and trading volume using historical market data (2013–2022).

## Overview
This project explores the long-term price behavior, volatility, and market cycles of Bitcoin using historical daily market data from 2013 to 2022. The analysis applies the full data science workflow — data cleaning, feature engineering, exploratory data analysis (EDA), and statistical interpretation — to better understand Bitcoin’s risk profile and boom-and-bust dynamics.

The goal of this project is to analyze how Bitcoin has evolved over time, how volatile it is compared to traditional assets, and how trading volume behaves during major market events.

## Dataset
- **Source:** Kaggle – Cryptocurrency Historical Prices  
- **Asset:** Bitcoin (BTC)  
- **Time Range:** April 29, 2013 → December 2022  
- **Observations:** 2,991 daily records  

**Key columns:**
- Date
- Open, High, Low, Close
- Volume
- Market Capitalization

## Data Preparation
The dataset was cleaned and prepared for time-series analysis:
- Converted date strings to `datetime` format and sorted chronologically
- Verified data completeness and removed any rows with missing OHLC values
- Engineered additional financial features to support deeper analysis

### Feature Engineering
New features include:
- Lagged closing price
- Daily returns
- Log returns
- 30-day rolling volatility (standard deviation of log returns)

These features enable analysis of volatility clustering and return distributions commonly observed in financial markets.

## Exploratory Data Analysis
The analysis focuses on several core areas:

### Bitcoin Price Over Time
- Early growth phase (2013–2016)
- 2017 bull market and subsequent crash
- 2020–2021 bull run to all-time highs
- 2022 bear market during macroeconomic tightening

### Volatility Analysis
- Distribution of daily returns shows heavy tails and non-normal behavior
- Rolling 30-day volatility highlights volatility clustering during both bull and bear markets

### Trading Volume Behavior
- Volume increases significantly during major price movements
- Spikes in volume coincide with periods of heightened speculation and market stress

## Research Questions Addressed
This project answers the following questions:
1. How has Bitcoin’s price changed over time?
2. How volatile is Bitcoin based on daily returns and rolling volatility?
3. How does trading volume behave during major price movements?
4. How does Bitcoin differ across bull and bear market regimes?
5. What patterns emerge from the distribution of daily returns?

## Key Findings
- Bitcoin exhibits a strong long-term upward trend with extreme volatility
- Volatility spikes during both euphoric bull markets and sharp market crashes
- Trading volume surges during major price movements
- Daily returns show heavy-tailed, non-normal distributions
- Market behavior differs significantly between bull and bear phases

## Technologies Used
- Python
- pandas
- NumPy
- matplotlib
- Jupyter Notebook

## Files in This Repository
- `bitcoin_price_analysis.ipynb` – Full analysis notebook
- `Bitcoin_Price_Analysis_Report.pdf` – Written report with interpretations and visuals
- `README.md` – Project overview and documentation

## Future Work
Potential extensions of this project include:
- Adding Ethereum and other cryptocurrencies for comparison
- Extending the dataset through 2023–2025
- Calculating risk metrics such as drawdowns and Value at Risk (VaR)
- Applying machine learning models for volatility prediction
- Incorporating macroeconomic indicators (CPI, interest rates, equity indices)

## Author
Roman Heath
