# Trader Performance vs Market Sentiment Analysis

## Overview

This project analyzes the relationship between **Bitcoin market sentiment (Fear & Greed Index)** and **trader behavior on the Hyperliquid exchange**.

The goal is to identify patterns between market sentiment and trader performance that could inform **smarter trading strategies and risk management decisions**.

The analysis combines two datasets:

1. **Bitcoin Market Sentiment Dataset** – Fear/Greed classification per day
2. **Historical Hyperliquid Trader Data** – Individual trade records including trade size, direction, and profit/loss

---

# Objective

The objective of this project is to investigate how **market sentiment influences trader behavior and performance** by analyzing:

* Trader profitability (PnL)
* Trading activity
* Position size
* Win rate
* Trader segmentation

The results aim to produce **actionable insights and strategy ideas** for improving trading performance under different market conditions.

---

# Datasets

### 1. Bitcoin Market Sentiment (Fear/Greed Index)

Contains daily classification of market sentiment.

**Columns include:**

* timestamp
* value
* classification (Fear / Greed / Extreme Fear / Extreme Greed)
* date

---

### 2. Hyperliquid Historical Trader Data

Contains detailed trade-level information.

**Columns include:**

* Account
* Coin
* Execution Price
* Size Tokens
* Size USD
* Side (Buy/Sell)
* Timestamp IST
* Direction
* Closed PnL
* Fee
* Trade ID

---

# Methodology

## 1. Data Preparation

The following preprocessing steps were performed:

* Loaded both datasets using pandas
* Checked dataset dimensions, duplicates, and missing values
* Converted timestamps into datetime format
* Created a **daily date column** for alignment
* Merged trading data with market sentiment data based on date

---

## 2. Feature Engineering

Several metrics were derived to support the analysis:

* **Daily trader PnL**
* **Win rate per trader**
* **Average trade size**
* **Number of trades per day**
* **Long vs Short trade ratio**
* **Trader segmentation**

  * Frequent vs Infrequent traders

---

## 3. Exploratory Data Analysis

The analysis focused on identifying relationships between **market sentiment and trader behavior** through:

* Profitability vs sentiment
* Trading activity vs sentiment
* Position size vs sentiment
* Win rate vs sentiment
* Trader segmentation performance

Visualizations were created using **Matplotlib and Seaborn**.

---

# Key Insights

### Insight 1 — Market Sentiment Influences Profitability

Average trader profitability varies across market sentiment categories.
Periods of **Extreme Greed tend to show higher profitability**, suggesting stronger market momentum.

---

### Insight 2 — Trading Activity Changes with Sentiment

Trading frequency increases during **Greed periods**, indicating that traders become more active when markets are bullish.

---

### Insight 3 — Frequent Traders Perform Better

Frequent traders demonstrate **higher average profitability and consistency**, suggesting experience and strategy refinement play an important role.

---

# Strategy Recommendations

### Strategy 1 — Reduce Risk During Fear Periods

During **Fear or Extreme Fear**, traders should reduce position sizes or leverage to mitigate downside volatility.

---

### Strategy 2 — Momentum Strategies During Greed

During **Greed or Extreme Greed**, traders may benefit from momentum-based strategies due to higher trading activity and market participation.

---

# Tools & Technologies

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Jupyter Notebook

---

# Repository Structure

```
trader-sentiment-analysis
│
├── trader_analysis.ipynb
├── README.md
└── charts
```

---

# How to Run the Project

1. Clone the repository

```
git clone https://github.com/yourusername/trader-sentiment-analysis
```

2. Install required libraries

```
pip install pandas numpy matplotlib seaborn
```

3. Open the notebook

```
jupyter notebook trader_analysis.ipynb
```

---

# Conclusion

This analysis demonstrates that **market sentiment significantly influences trader behavior and performance**.

Understanding sentiment-driven patterns can help traders optimize **risk management, position sizing, and trading frequency**, ultimately improving overall strategy performance.

---

# Author

Diya K D
