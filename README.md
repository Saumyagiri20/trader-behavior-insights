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

### Key Insights:
- Most trades occur during Greed periods
- Large trades tend to be more profitable than small ones
- Sentiment influences behavior, but does not guarantee profitability

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
