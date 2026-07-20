# 📈 Time Series Forecasting — A Beginner to Advanced Guide

> **Don't know what "time series" means? That's exactly who this is for.**
> This repository walks you through forecasting future values from historical data — in plain English, with hands-on Python notebooks.

---

## 🤔 What Is Time Series Forecasting? (In Plain English)

Imagine tracking your monthly electricity bill every month for 3 years. That list of numbers, recorded **over time**, is a **time series**.

**Forecasting** means using that history to answer: *"What will my bill be next month?"*

This kind of prediction is used everywhere:
- 📦 Amazon predicting product demand
- 💹 Banks forecasting stock prices
- ✈️ Airlines predicting passenger counts
- ⚡ Power companies estimating electricity usage

This repo teaches you how to do all of that — from scratch.

---

## 📁 Complete Repository Structure

```
Resource-Demand-Forecasting/
│
├── 📚 README.md (this file)
│
├── 📂 Basic Time Series Analysis Concepts/     ← START HERE! 20 comprehensive notebooks
│   ├── 1.  Intro to time series.ipynb
│   ├── 2.  Stationarity.ipynb
│   ├── 3.  Box-Cox Transform.ipynb
│   ├── 4.  Seasonality.ipynb
│   ├── 5.  Decomposition.ipynb
│   ├── 6.  Autocorrelation.ipynb
│   ├── 7.  Partial Autocorrelation.ipynb
│   ├── 9.  Basic Forecasting Techniques.ipynb
│   ├── 10. Simple Exponential Smoothing.ipynb
│   ├── 11. Holt's Linear Trend Model.ipynb
│   ├── 12. Holt Winters Forecasting.ipynb
│   ├── 13. Residuals.ipynb
│   ├── 14. Crossvalidation.ipynb
│   ├── 15. Autoregression.ipynb
│   ├── 16. Moving Average Models.ipynb
│   ├── 17. ARIMA.ipynb
│   ├── 18. SARIMA.ipynb
│   ├── 19. Fourier Series & Harmonic Regression.ipynb
│   └── AirPassengers.csv               ← Classic benchmark dataset
│
├── 📂 Implementation/                   ← Real-world applications
│   └── Brazilian_Logistics_Data(where_ARIMA_fails).ipynb
│       └── Practical case study showing ARIMA limitations on complex data
│
├── 📂 Dataset/                          ← Large-scale real datasets
│   └── Data_Vishnu.csv                  ← 46.9 MB resource demand data
│
├── 📂 MSTL Decomposition/               ← Advanced multi-seasonal techniques
│   ├── MSTL(using_electricity_dataset).ipynb
│   ├── Workforce_Forecasting(Version_1) (2).ipynb
│   ├── MSTL research paper.pdf          ← Original MSTL algorithm paper
│   └── prophet research paper.pdf       ← Facebook's Prophet forecasting tool
│
├── 📄 2207.03517v6.pdf                  ← Related research paper (~168 KB)
│
└── 🏗️ Hierarchical_Forecasting.ipynb    ← Advanced hierarchical forecasting methods
```

---

## 🗺️ Learning Path — Where to Start

Whether you're a complete beginner or someone brushing up, follow this path:

### 🟢 Complete Beginner
> No prior knowledge needed — just basic Python familiarity

1. **Notebook 1** → What is a time series? See your first plot.
2. **Notebook 2** → Stationarity — why data needs to be "stable" before forecasting
3. **Notebook 4** → Seasonality — patterns that repeat (like holiday sales every December)
4. **Notebook 5** → Decomposition — breaking data into trend + season + noise
5. **Notebook 9** → Your first basic forecast!

### 🟡 Intermediate
> You know Python and want to understand the models

6. **Notebook 10** → Simple Exponential Smoothing (weighted averages)
7. **Notebook 11** → Holt's model (handles trends)
8. **Notebook 12** → Holt-Winters (handles trends **and** seasons)
9. **Notebook 13** → Residuals (evaluating model performance)
10. **Notebook 14** → Cross-validation (proper model evaluation)
11. **Notebooks 15–16** → Autoregression & Moving Averages (the building blocks of ARIMA)
12. **Notebook 17** → ARIMA — the industry workhorse model
13. **Notebook 18** → SARIMA — ARIMA with seasonal awareness
14. **Notebook 19** → Fourier Series & Harmonic Regression

### 🔴 Advanced
> Ready for real-world complexity and cutting-edge techniques

15. **Box-Cox Transform (Notebook 3)** → Data transformation for better model performance
16. **Partial Autocorrelation (Notebook 7)** → Deep dive into ACF/PACF plots
17. **Implementation/** → See what happens when ARIMA breaks on messy logistics data
18. **Hierarchical_Forecasting.ipynb** → Forecasting with hierarchical data structures
19. **MSTL Decomposition/** → Multi-Seasonal decomposition for data with multiple seasonal patterns
    - Electricity dataset example (daily + weekly + yearly seasonality)
    - Workforce forecasting applications
20. **Research Papers** → Dive into MSTL and Prophet methodologies

---

## 🧠 Key Concepts Explained Simply

| Term | What It Means |
|------|--------------|
| **Stationarity** | The data's average and variability don't change over time. Models need this to work well. |
| **Seasonality** | A pattern that repeats at regular intervals — e.g., ice cream sales spike every summer. |
| **Trend** | The long-term direction — going up, going down, or flat. |
| **Decomposition** | Splitting a time series into its trend, seasonal, and random (residual) parts. |
| **Autocorrelation (ACF)** | How much today's value resembles yesterday's. High autocorrelation = very predictable data. |
| **Partial Autocorrelation (PACF)** | Autocorrelation after removing effects of intermediate lags. |
| **Exponential Smoothing** | Forecasting by giving more weight to recent data than older data. |
| **Residuals** | The difference between what the model predicted and what actually happened. Lower = better model. |
| **ARIMA** | A powerful statistical model combining past values (AR) and past errors (MA) with differencing (I). |
| **SARIMA** | ARIMA + seasonal patterns built in. |
| **Box-Cox Transform** | Mathematical transformation to stabilize variance and make data more suitable for modeling. |
| **Fourier Series** | Using sine and cosine functions to model complex seasonal patterns. |
| **Harmonic Regression** | Combining Fourier terms with regression for flexible seasonal modeling. |
| **MSTL** | Multi-Seasonal-Trend decomposition using LOESS — handles data with *multiple* seasonal cycles. |
| **Hierarchical Forecasting** | Forecasting with data organized in hierarchies (e.g., total sales → by region → by store). |
| **Cross-Validation** | Properly evaluating models without data leakage using time-series-aware techniques. |

---

## 📊 Datasets Included

| Dataset | Location | Size | Purpose |
|---------|----------|------|---------|
| `AirPassengers.csv` | Basic Time Series Analysis Concepts/ | 1.7 KB | Classic benchmark — monthly airline passengers (1949–1960) |
| `Data_Vishnu.csv` | Dataset/ | 46.9 MB | Large-scale resource demand forecasting data for real-world practice |
| Brazilian Logistics Data | Implementation/ | Embedded | Real freight/logistics time series — shows ARIMA's limitations |
| Electricity Dataset | MSTL Decomposition/ | Embedded | Hourly electricity consumption with multiple seasonal patterns |

---

## 📚 Research Papers & References

Three research papers are included for deeper learning:

- **MSTL Paper** (`MSTL Decomposition/`) — The original research on Multi-Seasonal-Trend decomposition using LOESS
- **Prophet Paper** (`MSTL Decomposition/`) — Facebook's forecasting tool designed for business time series with holidays and missing data
- **2207.03517v6.pdf** — Additional forecasting research paper

For hierarchical forecasting concepts, see: https://nixtlaverse.nixtla.io/hierarchicalforecast/

---

## 🛠️ How to Run the Notebooks

### 1. Clone the repository
```bash
git clone https://github.com/Vishnu912py/Resource-Demand-Forecasting.git
cd Resource-Demand-Forecasting
```

### 2. Install dependencies
```bash
pip install pandas numpy matplotlib scipy statsmodels scikit-learn jupyter
```

For advanced notebooks, also install:
```bash
pip install prophet statsmodels mstl
```

### 3. Launch Jupyter
```bash
jupyter notebook
```

Then open any `.ipynb` file in the `Basic Time Series Analysis Concepts/` folder and run cells top to bottom.

> 💡 **Tip:** Use [Google Colab](https://colab.research.google.com/) if you don't want to install anything locally — just upload the notebooks and run them in your browser for free.

---

## 📖 What Each Notebook Covers

### Basic Time Series Analysis Concepts

| # | Notebook | Key Topics |
|---|----------|-----------|
| 1 | Intro to time series | Time series definition, types of data, basic visualization |
| 2 | Stationarity | ADF test, making data stationary through differencing |
| 3 | Box-Cox Transform | Variance stabilization techniques |
| 4 | Seasonality | Identifying and quantifying seasonal patterns |
| 5 | Decomposition | Classical decomposition (additive/multiplicative) |
| 6 | Autocorrelation | ACF plots, interpreting autocorrelation |
| 7 | Partial Autocorrelation | PACF plots, identifying model orders |
| 9 | Basic Forecasting Techniques | Naive, seasonal naive, average methods |
| 10 | Simple Exponential Smoothing | Weighted averaging for forecasting |
| 11 | Holt's Linear Trend Model | Handling trends in time series |
| 12 | Holt-Winters Forecasting | Combined trend and seasonal forecasting |
| 13 | Residuals | Analyzing prediction errors for model diagnostics |
| 14 | Cross-validation | Proper time-series validation techniques |
| 15 | Autoregression | AR models and modeling with past values |
| 16 | Moving Average Models | MA models and handling error terms |
| 17 | ARIMA | Full ARIMA model implementation and tuning |
| 18 | SARIMA | Seasonal ARIMA for complex patterns |
| 19 | Fourier Series & Harmonic Regression | Advanced seasonal modeling techniques |

### Advanced Topics

| Notebook | Purpose |
|----------|---------|
| Hierarchical_Forecasting | Forecasting hierarchical data structures (total → regions → stores) |
| MSTL (Electricity) | Multi-seasonal decomposition on real electricity demand data |
| Workforce_Forecasting | Applying advanced techniques to workforce planning |
| Brazilian_Logistics | Real-world case: why ARIMA fails and alternative approaches |

---

## 💡 Common Questions

**Q: Do I need to be a math genius to understand this?**
> No. The notebooks focus on intuition and code. The math is there if you want it, but you can follow along without it.

**Q: What's the best model to use?**
> It depends on your data. Start with ARIMA for most cases. Use SARIMA if you have clear seasonal patterns. Use MSTL for complex, multi-layered seasonal data (like hourly readings). Use Hierarchical forecasting when your data has natural hierarchies.

**Q: Why does ARIMA "fail" on the Brazilian logistics data?**
> Real-world data is messy. The implementation notebook shows a case where the data has multiple overlapping patterns, missing values, and structural breaks that ARIMA can't handle well — and introduces better approaches like MSTL and hierarchical methods.

**Q: How do I choose between ARIMA, SARIMA, and MSTL?**
> - **ARIMA**: Simple trends, minimal seasonality
> - **SARIMA**: One clear seasonal pattern (e.g., monthly data with yearly seasonality)
> - **MSTL**: Multiple overlapping seasonal patterns (e.g., hourly data with daily AND weekly seasonality)

**Q: Can I use these models for my own data?**
> Yes! The notebooks teach reusable concepts. Replace the example datasets with your own CSV and follow the same workflow. Start with exploratory analysis, then try models in order of complexity.

---

## 🎯 Use Cases

This repository prepares you to forecast:
- 📦 **Inventory demand** — What products to stock
- 💼 **Resource allocation** — Workforce, server capacity, power consumption
- 💰 **Financial metrics** — Sales, revenue, stock prices
- 📊 **Operational data** — Website traffic, API requests, customer arrivals
- 🌡️ **Environmental data** — Temperature, pollution, weather patterns

---

## 📋 Skills You'll Gain

By completing this repository, you'll be able to:
- ✅ Recognize time series patterns (trend, seasonality, noise)
- ✅ Test and transform data for modeling
- ✅ Build and evaluate forecasting models
- ✅ Choose the right model for your data
- ✅ Handle real-world complexity (missing data, multiple seasons, hierarchies)
- ✅ Interpret model diagnostics and residual analysis
- ✅ Implement proper validation and backtesting

---

## ⭐ Like This Repo?

Give it a star ⭐ if you found it helpful — it helps others discover it too!

---

## 📝 License & Attribution

Created by [Vishnu912py](https://github.com/Vishnu912py)

*Made with 📚 + ☕ + 🧠*
