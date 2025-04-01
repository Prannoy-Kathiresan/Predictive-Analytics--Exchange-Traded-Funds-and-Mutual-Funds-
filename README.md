# 📈 Predictive Analysis of Exchange Traded Funds (ETFs) and Mutual Funds (MFs) Using R

This project analyzes and compares the predictive performance of Exchange-Traded Funds (ETFs) and Mutual Funds (MFs) using statistical modeling and machine learning techniques in R. It leverages a rich financial dataset scraped from Yahoo Finance to evaluate factors influencing fund returns and classification outcomes.

> 📁 Files included: `ETF and MF predictive analysis using R.Rmd` + Full Report (PDF)

---

## 🎯 Project Goals

- Identify key features influencing ETF and MF performance
- Predict fund returns using regression models
- Classify investment type and fund size using classification techniques
- Compare predictive power of ETFs vs. Mutual Funds

---

## 🧪 Statistical Methods Used

### 📊 Data Processing
- Cleaned and imputed missing values (e.g., ratios, returns, sectors)
- Categorized funds by size, type, and risk

### 📈 Regression Models
- Linear Regression
- Best Subset Selection
- KNN Regression
- Decision Trees (with cross-validation & pruning)
- Random Forest
- Ridge & Lasso Regression
- Gradient Boosting

**Best Performer**: Random Forest achieved the lowest MSE and highest R² (ETF R²: 82%, MF R²: 96.6%)

### 🧠 Classification
- Logistic Regression (for fund return prediction: High vs Low)
- Linear Discriminant Analysis (for fund size & investment type)

---

## 🔍 Key Insights

- ETFs are **more predictable** than MFs using available fund descriptors
- Growth ETFs outperform Growth MFs significantly in the long term
- Riskier MFs show high volatility but perform better short-term (1–3 years)
- ETF returns outperform MF returns beyond a 5-year horizon

---

## 📦 Dataset Description

- 2,310 ETFs and 23,783 Mutual Funds
- Features include:
  - Inception year, total assets, fund category
  - Portfolio composition (stocks, bonds, cash, sectors)
  - Historical returns (YTD, 1Y, 3Y, etc.)
  - Financial ratios (Sharpe, Treynor, Alpha, Beta)

---

## 📂 Project Files

- `ETF and MF predictive analysis using R.Rmd` — R Markdown code for full data pipeline
- `ETF and MF predictive analysis using R- Report.pdf` — Final report with detailed results, visuals, and methodology

---

## ⚙️ How to Run

1. Open the `.Rmd` file in RStudio
2. Knit to HTML or PDF
3. Required R packages:
```r
library(tidyverse)
library(randomForest)
library(caret)
library(glmnet)
library(MASS)
library(tree)
library(gbm)
library(leaps)
```

---

## 📬 Contact

Have questions or ideas? Reach out via [LinkedIn](https://www.linkedin.com/in/prannoy-k)

---

## 📚 References

- Yahoo Finance dataset (scraped)
- STAT432: Basics of Statistical Learning – UIUC
- Elements of Statistical Learning (Hastie, Tibshirani, Friedman)
