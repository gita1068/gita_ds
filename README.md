# Trader Behavior vs Market Sentiment Analysis

## Problem Statement
This analysis explores how trader behavior on Hyperliquid varies across different Bitcoin market sentiment regimes (Fear vs Greed), with a focus on profitability, risk-taking, and trade activity.

## Datasets
- Historical Trader Data (211k+ trades): Includes trade size, execution price, fees, and realized PnL.
- Bitcoin Fear & Greed Index (daily): Captures overall market sentiment states.

## Methodology
- I converted intraday trade data into daily trader-level aggregates to align with daily sentiment data.
- Daily trader behavior was mapped to the corresponding market sentiment.
- Traders were segmented into Top 20% and Bottom 20% based on cumulative PnL.
- Behavioral patterns were compared across different sentiment regimes.

## Key Insights
- Trade activity peaks during Fear, indicating reactive behavior.
- Increased activity during Fear does not translate into higher realized PnL.
- Top traders maintain consistent participation across all sentiment regimes.
- Bottom traders tend to overtrade during Fear and under-participate during Greed.

## Strategic Implications
- Market sentiment should be used as a risk filter rather than a direct trading signal.
- Trading systems should limit impulsive trade frequency during Fear phases.
- Consistent, disciplined participation outperforms sentiment-driven reactivity.

## Limitations
- Closed PnL is only recorded when positions are exited, which may underrepresent intraday profitability.
- Leverage data was unavailable in the dataset, limiting risk-adjusted analysis.

## Next Steps
- Incorporate leverage-adjusted performance metrics.
- Analyze sentiment lag effects on trader behavior.
- Backtest sentiment-aware risk control strategies.

## Data Availability Note
The full historical trader dataset exceeds GitHub’s file size limits and is therefore not included in this repository.  
The dataset can be accessed using the official link provided in the assignment instructions.

All analysis was performed in Google Colab using the original dataset.



