# Financial News Sentiment & Stock Price Analysis

**Client:** Nova Financial Solutions  
**Subject:** Task 1-3 Completion (EDA, Quantitative Analysis, and Sentiment Correlation)

---

## 📊 Project Overview

This repository contains a comprehensive data pipeline designed to analyze the impact of financial news sentiment on stock price movements. Using **AAPL** as a primary case study, we integrated natural language processing (NLP) with technical financial indicators to uncover potential trading edges.

---

## 📂 Repository Structure

* **`notebooks/eda_news.ipynb`**: Exploratory Data Analysis of the news dataset, including publication trends and headline length statistics.
* **`notebooks/stock_analysis.ipynb`**: Implementation of technical indicators (SMA, EMA, RSI, MACD, and Bollinger Bands) to quantify price volatility and momentum.
* **`notebooks/sentiment_analysis.ipynb`**: Statistical correlation between VADER sentiment scores and daily Log Returns.
* **`data/raw/`**: Storage for the raw financial datasets.

---

## 🛠️ Key Technical Implementations

### **1. Sentiment Analysis**
Utilized the **VADER (Valence Aware Dictionary and sEntiment Reasoner)** lexicon to quantify the emotional tone of thousands of headlines. Scores were aggregated daily to match trading session windows.

### **2. Quantitative Indicators**
* **Bollinger Bands**: Used to visualize price volatility and identify "overbought" or "oversold" conditions.
* **RSI & MACD**: Integrated momentum oscillators to determine the strength of price trends.
* **Log Returns**: Calculated daily returns using $\ln(P_t / P_{t-1})$ for statistical normalization.

### **3. Correlation & Insights**
* Calculated **Pearson Correlation Coefficient ($r$)** and **P-values** to test the significance of news impact.
* **Categorical Analysis**: Discovered that while raw daily correlation is low, there is a measurable divergence in average returns between "Positive" and "Negative" news days.

---

## 📈 Summary of Findings

* **Market Efficiency**: The low linear correlation suggests that financial markets price in news sentiment very rapidly.
* **Strategic Edge**: Categorical grouping proves that sentiment acts as a significant secondary filter for risk management. High-sentiment days correlate with stabilized positive returns, whereas low-sentiment days exhibit higher downward volatility.

---

## 🚀 Setup and Installation

1. **Clone the repository**:
   ```bash
   git clone [https://github.com/YOUR_USERNAME/YOUR_REPO.git](https://github.com/YOUR_USERNAME/YOUR_REPO.git)

2. Install dependencies:

pip install pandas numpy yfinance pandas_ta nltk matplotlib seaborn scipy
Run the Analysis: Open the notebooks in the notebooks/ directory using Jupyter or VS Code.

3. Run the Analysis: Open the notebooks in the notebooks/ directory using Jupyter or VS Code.

### **Pro Tip for VS Code:**
To see what it will actually look like while you are editing, press **`Ctrl + Shift + V`** (Windows) or **`Cmd + Shift + V`** (Mac). This opens the **Markdown Preview** window so you can check the formatting before you push it to GitHub!