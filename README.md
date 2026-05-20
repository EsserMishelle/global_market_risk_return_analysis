# Global Market Risk Return Analysis

## Project Overview
This analysis analyzes global market performance, volatility, and risk-adjusted efficiency across major asset classes using financial market data. It combines exploratory data analysis in Python with executive-style dashboarding in Tableau to evaluate return behavior, market sentiment, and investment efficiency across multiple investment horizons.

The project focuses on key financial indicators including return performance, Sharpe ratios, volatility, composite scoring, and Fear-Greed sentiment metrics. Since several financial indicators contained substantial missing values, the final executive analysis emphasizes broader asset-class behavior rather than detailed sector-level modeling.

## Dataset
The Kaggle dataset is collected directly from Yahoo Finance and enriched with production-grade technical indicators, fundamental ratios, and proprietary composite scores. The dataset at a glance includes 451 tickers, 131 columns, and 8 asset classes. It provides one year of price history spanning April 2025 to April 2026, sourced from Yahoo Finance via yfinance. Market capitalizations have been normalized to USD, and the dataset is released under a CC0 Public Domain license.

The original dataset is attached below:

[Original Dataset](https://github.com/EsserMishelle/global_market_risk_return_analysis/blob/main/yahoo_finance_global_markets_2026.csv)

## Exploratory Data Analysis (EDA)
Initial exploratory analysis focused on evaluating missing values, feature distributions, correlations, and market behavior across return, volatility, and sentiment metrics. Several sector- and industry-level variables contained substantial missing values, making asset-class level analysis more appropriate for executive dashboarding and comparative market evaluation.

### Correlation Analysis
Correlation analysis revealed strong relationships between longer-term return horizons and Sharpe efficiency metrics, while volatility indicators demonstrated strong internal correlation across time periods.

## Jupyter Notebook Analysis
The complete techincal exploratory analysis, feature engineering, correlation analysis, and csv file export (for Tableau) workflow were developed in Python using Jupyter Notebook.

[Jupyter Notebook Analysis]

## Feature Engineering and Selected Metrics
The final executive analysis focused on financial indicators most relevant to market performance, risk evaluation, and executive decision-making:

Return Horizons (1M, 6M, 1Y)
1-Year Volatility
Sharpe Ratio
Composite Score
Fear-Greed Sentiment
Market Capitalization
Momentum Indicators
Risk-Adjusted Rankings

These metrics were selected to balance return performance, market risk, sentiment behavior, and overall investment efficiency across global asset classes. These selected features were exported as a CSV file for executive visualization in Tableau.

## Tableau 
The final executive dashboard was developed in Tableau Public to provide an interactive view of global market performance, risk-adjusted efficiency, sentiment distribution, and composite scoring across major asset classes and sectors. The dashboard combines return horizons, Sharpe analysis, market sentiment, and composite performance metrics to support executive-level market evaluation and comparative investment analysis.

Tableau Public Dashboard:

[Interactive Tableau Public Dashboard]
[Global Market Risk Return Analysis](https://github.com/EsserMishelle/global_market_risk_return_analysis/blob/main/Global_Market_Risk_Return_Analysis.twbx)

# Project Files
[GitHub Repoistory]

# Conclusion
International and ETF markets demonstrated the strongest long-term risk-adjusted performance, while Crypto remained the weakest and most volatile asset class across multiple investment horizons. Composite scoring and sentiment analysis further highlighted stronger market concentration within diversified global equity markets relative to higher-volatility alternative assets.

