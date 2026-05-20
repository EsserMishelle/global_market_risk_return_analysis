<img width="1048" height="585" alt="pexels-pixabay-534216" src="https://github.com/user-attachments/assets/b200948e-9c20-454e-b868-71546add925d" />

# Global Market Risk Return Analysis

## Project Overview
This analysis analyzes global market performance, volatility, and risk-adjusted efficiency across major asset classes using financial market data. It combines exploratory data analysis in Python with executive-style dashboarding in Tableau to evaluate return behavior, market sentiment, and investment efficiency across multiple investment horizons.

The project focuses on key financial indicators including return performance, Sharpe ratios, volatility, composite scoring, and Fear-Greed sentiment metrics. Since several financial indicators contained substantial missing values, the final executive analysis emphasizes broader asset-class behavior rather than detailed sector-level modeling.

## Dataset
The Kaggle dataset is collected directly from Yahoo Finance and enriched with production-grade technical indicators, fundamental ratios, and proprietary composite scores. The dataset at a glance includes 451 tickers, 131 columns, and 8 asset classes. It provides one year of price history spanning April 2025 to April 2026, sourced from Yahoo Finance via yfinance. Market capitalizations have been normalized to USD, and the dataset is released under a CC0 Public Domain license.

The screenshots display a partial preview of the orginal dataset.  

<img width="1837" height="340" alt="image" src="https://github.com/user-attachments/assets/1b4cf2b4-c9e1-4c21-9492-c546ad8c7b17" />
<img width="1875" height="341" alt="image" src="https://github.com/user-attachments/assets/e6a1fed8-420a-4ba9-bb9d-c020ea6285c3" />

The original dataset is attached below:

[Original Dataset](https://github.com/EsserMishelle/global_market_risk_return_analysis/blob/main/yahoo_finance_global_markets_2026.csv)

## Technogies Used
- Python
- Pandas
- NumPy
- Seaborn
- Matplotlib
- Tableau
- Jupyter Notebook
  
## Exploratory Data Analysis (EDA)
Initial exploratory analysis focused on evaluating missing values, feature distributions, correlations, and market behavior across return, volatility, and sentiment metrics. Several sector- and industry-level variables contained substantial missing values, making asset-class level analysis more appropriate for executive dashboarding and comparative market evaluation.

### Correlation Analysis

Heapmap Chart
<img width="939" height="590" alt="image" src="https://github.com/user-attachments/assets/d91abbe4-7219-4526-a938-880537caeb6e" />

Correlation analysis revealed strong relationships between Momentum Score, Composite Score, and medium- to long-term return horizons, suggesting that assets with sustained upward momentum also demonstrated stronger overall investment quality and performance consistency. 

Momentum Score showed especially high correlation with 3-month (0.91) and 6-month (0.97) returns and Market Cap USD (0.85), while Composite Score aligned closely with both Sharpe efficiency and longer-term return performance.

Fear-Greed sentiment displayed an inverse relationship with volatility metrics (-0.73 ~ -0.82), indicating that higher market optimism generally corresponded with lower observed market risk across asset classes.

Longer-term returns demonstrate stronger positive relationships with Sharpe ratios, particularly between 1-Year Return and 1-Year Sharpe (0.75), indicating that stronger long-term performance is generally associated with improved risk-adjusted efficiency. 

Volatility measures also exhibit strong internal correlation, especially between 90-Day and 1-Year Volatility (0.89), while showing weaker or negative relationships with Sharpe performance. Overall, the analysis suggests that long-term return consistency contributes more strongly to market efficiency than short-term market fluctuations.

## Jupyter Notebook Analysis
The complete techincal exploratory analysis, feature engineering, correlation analysis, and csv file export (for Tableau) workflow were developed in Python using Jupyter Notebook.

[Jupyter Notebook Analysis](https://github.com/EsserMishelle/global_market_risk_return_analysis/blob/main/global_market_risk_return_analysis.ipynb)

## Feature Engineering and Selected Metrics
The final executive analysis focused on financial indicators most relevant to market performance, risk evaluation, and executive decision-making:

Selected features included return horizons, volatility measures, risk-adjusted efficiency metrics, momentum indicators, market sentiment signals, composite scoring models, ranking systems, and market capitalization data across multiple asset classes and sectors.

The curated Tableau export also retained supporting market metadata, pricing history, technical indicators, and classification attributes to support interactive filtering, comparative analysis, and dashboard storytelling.

## Tableau 
The final executive dashboard was developed in Tableau Public to provide an interactive view of global market performance, risk-adjusted efficiency, sentiment distribution, and composite scoring across major asset classes and sectors. The dashboard combines return horizons, Sharpe analysis, market sentiment, and composite performance metrics to support executive-level market evaluation and comparative investment analysis.

<img width="1187" height="887" alt="image" src="https://github.com/user-attachments/assets/595a2c68-98c0-49b2-b12d-7edaa8e5f0dc" />

Tableau Public Dashboard:

[Interactive Tableau Public Dashboard]

[Global Market Risk Return Analysis](https://github.com/EsserMishelle/global_market_risk_return_analysis/blob/main/Global_Market_Risk_Return_Analysis.twbx)

## Project Folder
[GitHub Repoistory](https://github.com/EsserMishelle/global_market_risk_return_analysis)

## Key Findings
- International and ETF markets demonstrated the strongest long-term risk-adjusted performance.
- Crypto exhibited the highest volatility and weakest return stability across investment horizons.
- Momentum leadership became increasingly concentrated within Energy and International sectors.
- Fear-Greed sentiment analysis revealed stronger bullish concentration across diversified equity markets.

# Conclusion
- International and ETF markets exhibit the strongest risk-adjusted performance Crypto remained the weakest and most volatile asset class across multiple horizons.

- Diversified global markets demonstrated stronger long-term efficiency and stability than higher-volatility assets.

- Market performance varied significantly across asset classes, indicating the importance of balancing return with volatility.

- Composite and momentum analysis further revealed leadership concentration within Energy, Utilities, and diversified international sectors, while several US Mid and speculative asset groups exhibited weakening momentum and higher return instability.

