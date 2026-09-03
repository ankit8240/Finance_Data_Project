# 📊 Finance Data Analysis Project

An exploratory and in-depth **financial data analysis project** focused on analyzing the stock performance of major U.S. banks using Python, Pandas, NumPy, Matplotlib, Seaborn, and financial-data APIs.

The project demonstrates how financial market data can be collected, processed, analyzed, and visualized to understand **stock performance, returns, volatility, risk, correlations, moving averages, and market behavior**.



---

## 📌 Project Overview

The project analyzes major U.S. bank stocks and explores their performance over different periods.

The analysis includes:

* 📈 Stock price analysis
* 💰 Daily and cumulative returns
* 📊 Risk and volatility analysis
* 🔗 Correlation analysis
* 📦 Return distributions
* 📉 Moving averages
* 🕯️ OHLC and candlestick analysis
* 📊 Trading volume analysis
* 🌎 Market-phase performance
* 🦠 COVID-19 market crash analysis
* 📐 Risk vs. return comparison

---

## 🏦 Banks Analyzed

The project works with the following bank stocks:

| Bank            | Ticker |
| --------------- | ------ |
| JPMorgan Chase  | `JPM`  |
| Bank of America | `BAC`  |
| Citigroup       | `C`    |
| Wells Fargo     | `WFC`  |
| Goldman Sachs   | `GS`   |
| Morgan Stanley  | `MS`   |

---

## 🛠️ Technologies Used

* **Python**
* **Jupyter Notebook**
* **Pandas** – Data manipulation and analysis
* **NumPy** – Numerical computations
* **Matplotlib** – Data visualization
* **Seaborn** – Statistical visualization
* **yfinance** – Financial market data
* **pandas-datareader** – Financial data retrieval
* **Plotly**
* **Cufflinks**

---

## 📂 Project Structure

```text
Finance-Project/
│
├── 03-Finance Project.ipynb
├── fin.ipynb
└── README.md
```

### 📓 `03-Finance Project.ipynb`

The original exploratory analysis focuses on bank stocks during the **2006–2016 period**, including the 2007–08 financial crisis.

It covers:

* Stock data collection
* Daily returns
* Best and worst daily returns
* Return distributions
* Standard deviation
* Correlation analysis
* Moving averages
* Heatmaps
* Candlestick charts
* Bollinger Bands
* Technical analysis

The notebook uses `pandas-datareader` for financial data retrieval.

### 📓 `fin.ipynb`

The expanded analysis examines major U.S. banks from **2015–2024**.

It includes:

* Closing price and volume analysis
* Cumulative returns
* Daily return distributions
* Annualized return and volatility
* Risk vs. return analysis
* OHLC analysis
* COVID-19 crash analysis
* Pre-COVID, COVID-crash, and post-COVID performance

---

## 📊 Key Analysis

### 1. Stock Price Analysis

Historical stock prices are analyzed to understand long-term price movements and trends.

### 2. Daily Returns

Daily percentage returns are calculated using:

```python
daily_returns = closing_prices.pct_change().dropna()
```

This helps measure day-to-day changes in stock prices.

### 3. Cumulative Returns

Cumulative returns are used to compare how a hypothetical investment would have grown over the analysis period.

```python
cumulative_returns = (1 + daily_returns).cumprod()
```

### 4. Risk & Volatility

The project calculates annualized return and volatility to compare the risk-return characteristics of different banks.

```python
Annualized Return = daily_returns.mean() * 252
Annualized Volatility = daily_returns.std() * np.sqrt(252)
```

### 5. Correlation Analysis

Correlation matrices and heatmaps are used to examine relationships between bank stock prices.

### 6. Market-Phase Analysis

The project compares performance across:

* Pre-COVID period
* COVID-19 market crash
* Post-COVID recovery

---

## 📈 Visualizations

The project uses several visualization techniques, including:

* Line charts
* Box plots
* Scatter plots
* Heatmaps
* Cluster maps
* OHLC charts
* Candlestick charts
* Moving-average charts
* Bollinger Band charts
* Trading-volume charts

---

## ⚙️ Installation

### 1. Install Python

Install Python from the official Python website or use **Anaconda**.

### 2. Install Required Libraries

Open the terminal in VS Code and run:

```bash
pip install pandas numpy matplotlib seaborn yfinance pandas-datareader plotly cufflinks
```

### 3. Launch Jupyter Notebook

```bash
jupyter notebook
```

Then open either:

```text
03-Finance Project.ipynb
```

or

```text
fin.ipynb
```

---

## 🚀 How to Run

1. Clone this repository:

```bash
git clone git@github.com:ankit8240/Finance-Project.git
```

2. Open the project folder in **VS Code**.

3. Install the required Python libraries.

4. Open the `.ipynb` notebook.

5. Select your Python/Jupyter kernel.

6. Run the notebook cells sequentially.

> **Note:** Financial data is retrieved from online data sources, so an active internet connection may be required when running the data-acquisition cells.

---

## 🎯 Learning Objectives

This project helps demonstrate practical skills in:

* Data collection
* Data cleaning
* Exploratory Data Analysis (EDA)
* Financial data analysis
* Pandas DataFrames
* Statistical analysis
* Data visualization
* Time-series analysis
* Return calculations
* Risk analysis
* Correlation analysis
* Python-based financial analytics

---

## 🔍 Project Insights

The analysis demonstrates that:

* Bank stocks can have significantly different risk and return characteristics.
* Major market events can strongly affect the banking sector.
* Bank stocks often show substantial correlation with one another.
* Volatility is an important factor when comparing stock performance.
* Market conditions can significantly change the performance of financial stocks.

---



⭐ If you found this project useful, consider giving the repository a **star**!
