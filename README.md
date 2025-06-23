# Trader Behavior Insights Based on Bitcoin Market Sentiment

This project explores the relationship between trader performance and Bitcoin market sentiment (Fear/Greed). By combining historical trader execution data with the Bitcoin Fear & Greed Index, we aim to uncover behavioral trends and strategies for smarter crypto trading.

## Dataset Overview

### 1. Bitcoin Fear & Greed Index
- Columns: `timestamp`, `value`, `classification`, `date`
- Description: Measures overall market sentiment — either Fear or Greed

### 2. Trader Data from Hyperliquid
- Columns: `Account`, `Coin`, `Execution Price`, `Size USD`, `Side`, `Timestamp`, `Closed PnL`, etc.
- Description: Records of trade executions including size, direction, and PnL


## Methods and Features

- Timestamp Parsing: Unix timestamps converted to readable dates
- Dataset Merging: Joined on `Date` field
- Feature Engineering:
  - `profitable` flag based on `Closed PnL`
  - `size_category`: Small / Medium / Large (based on USD value)
  - `trade_direction`: Buy/Sell behavior


## Exploratory Data Analysis (EDA)

## Key Insights

- Most trades occur during periods of market "Greed."
- While small trades are more frequent, larger trades tend to yield higher profits.
- Traders behave differently during "Fear" vs "Greed" phases, indicating sentiment-driven strategies.
- Sentiment alone does not guarantee profitability.



## Most Important Insights (Highlights)

1. **Majority of Trades Occur During "Greed" Sentiment**  
   Traders are more active during Greed phases, showing behavioral influence of positive sentiment.

2. **Large Trades Are More Likely to Be Profitable**  
   Bigger trades, though fewer, generate more consistent profits — often tied to experienced participants.

3. **"Fear" Periods Reduce Activity and Profitability**  
   Trading still happens, but in a more cautious and less profitable manner.

4. **Sentiment ≠ Profitability**  
   Emotional state influences behavior — not financial outcome.

5. **Small Trades Dominate in Volume But Not in Value**  
   High volume of low-impact trades may point to beginner or retail trading patterns.



### Visuals:
- Profitability by sentiment (Fear/Greed)
- Trade size vs profitability
- Trade count distribution across sentiment types


## Files

| File Name                    | Description                              |
|-----------------------------|------------------------------------------|
| `Assigment.ipynb`           | Final cleaned Jupyter Notebook           |
| `trader_sentiment_merged.csv` | Preprocessed data file for reference |
| `README.md`                 | Project overview file                    |


## Author

Name: Saumya Giri  
LinkedIn: [https://www.linkedin.com/in/saumya-giri-782ab2251/](https://www.linkedin.com/in/saumya-giri-782ab2251/)  
GitHub: [https://github.com/Saumyagiri20](https://github.com/Saumyagiri20)  
