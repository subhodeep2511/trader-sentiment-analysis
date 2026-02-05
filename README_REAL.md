# Trader Performance vs Market Sentiment

## Overview
This project analyzes how Bitcoin market sentiment (Fear & Greed Index) relates to trader behavior and performance on the Hyperliquid platform.

## Data
- Bitcoin Fear & Greed Index (daily sentiment classification)
- Hyperliquid historical trader data (executions, PnL, trade size, direction)

## Methodology
- Cleaned and aligned both datasets at a daily level
- Engineered performance and behavior metrics (PnL, trade frequency, position size)
- Used trade size as a proxy for risk exposure due to missing account balance data
- Segmented traders by risk level and analyzed behavior across sentiment regimes

## Key Insights
- Market sentiment amplifies risk: aggressive traders benefit most during Greed but face unstable outcomes during Fear.
- High average returns among high-risk traders come with higher volatility and loss frequency.
- Traders increase trade frequency and position size during Greed regimes.

## Strategy Recommendations
- Reduce position size or leverage during Fear and Extreme Fear regimes for high-risk traders.
- Enable aggressive strategies selectively during Greed regimes for traders with positive historical performance.

## How to Run
```bash
pip install pandas numpy matplotlib seaborn scikit-learn
jupyter notebook notebooks/analysis.ipynb
    