# Trader Performance vs Market Sentiment Analysis

## Overview
This project analyzes how market sentiment (Fear/Greed Index) affects trader behavior and performance using historical trading data. The objective is to identify behavioral patterns, evaluate performance across sentiment regimes, and derive actionable trading insights.

---

## Dataset

### Market Sentiment (Fear/Greed Index)
- timestamp
- date
- value (0–100)
- classification (Extreme Fear, Fear, Neutral, Greed, Extreme Greed)

### Historical Trader Data
- Account
- Coin
- Execution Price
- Size Tokens
- Size USD
- Side
- Direction
- Closed PnL
- Fee
- Trade ID
- Order ID
- Start Position
- Crossed
- Transaction Hash
- Timestamp IST
- Timestamp

---

## Methodology

### Data Preparation
- Cleaned datasets (no missing/duplicates)
- Converted timestamps to daily level
- Merged datasets using common date range
- Created daily trading metrics

### Feature Engineering
- Daily PnL
- Number of trades per day
- Average trade size
- Win rate
- Long/Short ratio
- Trader segmentation (Frequent vs Infrequent, Consistent vs Inconsistent)

### Analysis
- Compared performance across sentiment regimes
- Studied behavior change (activity, trade size, volatility)
- Identified trader segments

### Bonus
- Logistic Regression model to predict next-day profitability
- Lightweight Gradio dashboard for interactive exploration

---

## Key Insights

- Traders earn highest profits during Fear regimes.
- Trading activity increases during volatile periods.
- Consistent traders outperform aggressive traders.
- Larger trade sizes reduce profit stability.

---

## Strategy Recommendations

**Strategy 1 — Volatility Exploitation (Fear Regime)**
Increase trade frequency during Fear while controlling position size.

**Strategy 2 — Risk Control (Greed Regime)**
Reduce trading activity during Greed and focus on high-probability setups.

---

## Bonus Conclusion
Logistic Regression achieved ~73% accuracy, indicating trader profitability is partially predictable using sentiment and behavior.

---

## How to Run

Install dependencies:
pip install pandas numpy matplotlib seaborn scikit-learn
Run notebook or script:
Trader_Sentiment_Analysis.ipynb
(Optional) Run dashboard:
gradio_dashboard.ipynb
Run notebook:
Trader_Sentiment_Analysis.ipynb
Run dashboard (optional): GRADIO THAT IS IN THE NOTEBOOK FILE


---

## Author
RISHAV KUMAR SINGH
