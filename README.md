# Trader Performance vs Market Sentiment Analysis

## Primetrade.ai – Data Science Intern Round-0 Assignment

### Objective

The objective of this project is to analyze the relationship between Bitcoin market sentiment (Fear vs. Greed) and trader behavior on Hyperliquid. By combining historical trading data with the Bitcoin Fear & Greed Index, this analysis identifies patterns in trader profitability, trading activity, and market behavior, and proposes actionable trading strategies.

---

## Dataset

### 1. Bitcoin Fear & Greed Index
- Fields: Timestamp, Value, Classification, Date
- Sentiment categories include Fear, Greed, Neutral, and Extreme Greed.

### 2. Hyperliquid Historical Trades
Contains trading information such as:
- Account
- Coin
- Execution Price
- Trade Size
- Direction
- Closed PnL
- Fee
- Timestamp
- Transaction Details

---

## Project Structure

```
Primetrade_Assignment/

│
├── data/
│   ├── fear_greed_index.csv
│   └── historical_data.csv
│
├── notebooks/
│   └── analysis.ipynb
│
├── outputs/
│   └── charts/
│       ├── pnl_by_sentiment.png
│       ├── trade_frequency.png
│       ├── average_trade_size.png
│       ├── long_short_ratio.png
│       ├── pnl_distribution.png
│       └── top10_traders.png
│
├── README.md
└── requirements.txt
```

---

## Methodology

The analysis was performed in the following stages:

1. Data Loading
2. Data Cleaning and Inspection
3. Timestamp Conversion and Dataset Alignment
4. Feature Engineering
5. Exploratory Data Analysis
6. Trader Segmentation
7. Insight Generation
8. Strategy Recommendations

---

## Features Engineered

- Daily Trading Date
- Win/Loss Indicator
- Average Closed PnL
- Average Trade Size
- Trading Frequency
- Long vs Short Distribution
- Trader Performance Summary

---

## Analysis Performed

The notebook investigates the following questions:

- Does trader profitability differ between Fear and Greed market conditions?
- Does market sentiment influence trading activity?
- Does market sentiment affect average trade size?
- Do traders change their Long/Short behavior during different market conditions?
- Which traders generate the highest cumulative profits?

---

## Key Findings

- Market sentiment influences both trader activity and profitability.
- Trading behavior changes across different sentiment regimes.
- Trader profitability is unevenly distributed, with a relatively small group of traders generating a significant portion of cumulative profits.
- Market sentiment can be incorporated into trading risk management and decision-making.

---

## Sample Visualizations

The following visualizations highlight key insights from the analysis.

### Average Closed PnL by Market Sentiment

![Average Closed PnL](outputs/charts/pnl_by_sentiment.png)

---

### Trading Activity by Market Sentiment

![Trade Frequency](outputs/charts/trade_frequency.png)

---

### Average Trade Size by Market Sentiment

![Average Trade Size](outputs/charts/average_trade_size.png)

---

### Long vs. Short Position Distribution

![Long vs Short Ratio](outputs/charts/long_short_ratio.png)

---

### Distribution of Closed PnL

![PnL Distribution](outputs/charts/pnl_distribution.png)

---

### Top 10 Traders by Total Closed PnL

![Top 10 Traders](outputs/charts/top10_traders.png)

---

## Strategy Recommendations

- Apply more conservative position sizing during Fear periods.
- Use market sentiment as an additional risk-management signal rather than a standalone trading indicator.
- Adapt trading exposure according to historical trader performance.

---

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- SciPy
- Jupyter Notebook

---

## How to Run

### 1. Clone the repository

```bash
git clone https://github.com/Abhilasha-git/primetrade-assignment.git
```

### 2. Navigate to the project directory

```bash
cd primetrade-assignment
```

### 3. Install the required dependencies

```bash
pip install -r requirements.txt
```

### 4. Launch Jupyter Notebook

```bash
cd notebooks
jupyter notebook analysis.ipynb
```

### 5. Run the analysis

Open **analysis.ipynb** and run all cells sequentially (**Kernel → Restart & Run All**) to reproduce the complete analysis, summary tables, and visualizations.

---

## Repository Contents

- `analysis.ipynb` – Complete analysis notebook
- `outputs/charts/` – Visualizations generated during the analysis
- `README.md` – Project documentation
- `requirements.txt` – Python dependencies

---

## Conclusion

This project demonstrates how market sentiment can provide valuable context for understanding trader behavior. Integrating behavioral indicators such as the Fear & Greed Index with historical trading data can support more informed trading strategies and improve risk management decisions.