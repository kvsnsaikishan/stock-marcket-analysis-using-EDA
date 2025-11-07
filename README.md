# stock-marcket-analysis-using-EDA

# 📈 Yahoo Finance EDA Project  
### Stock Market Analysis – TCS | Wipro | Infosys | Capgemini  

---

## 🧰 Tools & Technologies
- **Python**
- **yFinance**
- **Pandas**
- **Matplotlib**
- **NumPy**
- **Jupyter Notebook**

---

## 🧩 Project Overview
This project performs an **Exploratory Data Analysis (EDA)** on leading IT companies using **Yahoo Finance data** over the past 10 years.  
It covers price trends, trading volume, and performance insights through **data visualization and resampling** (monthly, yearly).

---

## ⚙️ Steps Performed

### 1️⃣ Install Dependencies
```bash
pip install yfinance pandas matplotlib numpy
```

### 2️⃣ Import Core Libraries
```python
import yfinance as yf
import pandas as pd
import matplotlib.pyplot as plt
```

### 3️⃣ Define Company Tickers
```python
companies = ['TCS.NS', 'WIPRO.NS', 'INFY.NS', 'CAPGEMINI.PA']
```

### 4️⃣ Set Date Range (10 Years)
```python
start_date = "2015-01-01"
end_date = "2025-01-01"
```

### 5️⃣ Fetch Data
```python
data = {ticker: yf.download(ticker, start=start_date, end=end_date) for ticker in companies}
```

### 6️⃣ Data Summary & Cleaning
- Checked for missing values and null data  
- Computed descriptive statistics  
- Renamed columns for consistency  

### 7️⃣ Resampling (Monthly & Yearly)
- Monthly high, low, and close prices  
- Annual volume summaries  
- Comparative trend visualization  

---

## 📊 Key Insights

### 🔹 TCS
- Consistent growth between **2015–2025**
- Major peak during **2021–2024 tech boom**
- Stable long-term momentum despite small 2025 correction

### 🔹 Wipro
- Hit highest valuation between **2021–2022**
- Slight decline post-2023 but above pre-COVID levels
- Trading volume peaked in **2020**

### 🔹 Infosys & Capgemini
- Similar bullish trends to TCS, with strong recovery post-2020  
- 2024 showed stable consolidation phase  

---

## 📉 Visualizations
Includes multiple line plots for:
- Monthly High / Low / Adjusted Close  
- Yearly Volume Trends  
- Comparative Stock Movements  

---

## 🧠 Learnings
- Gained insights into **financial data handling using Python**
- Learned **time series resampling and visualization**
- Understood **stock volatility and growth patterns** across IT companies  

---

## 🗂️ Folder Structure
```
YAHOO_FINANCE_EDA_PROJECT/
│
├── YAHOO_FINANCE_EDA_PROJECT.ipynb
├── data/
│   └── (auto-downloaded from yFinance)
└── README.md
```

---

## 🚀 Future Scope
- Add **machine learning models** for stock price prediction  
- Integrate with **Streamlit dashboard** for real-time visualization  
- Compare IT sector performance vs NIFTY index  
