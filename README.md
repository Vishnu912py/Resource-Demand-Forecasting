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

## 📁 What's Inside This Repository

```
time_series_forecasting/
│
├── 📂 Basic Time Series Analysis Concepts/   ← Start here!
│   ├── 1.  Intro to Time Series
│   ├── 2.  Stationarity
│   ├── 3.  Box-Cox Transform
│   ├── 4.  Seasonality
│   ├── 5.  Decomposition
│   ├── 6.  Autocorrelation
│   ├── 7.  Partial Autocorrelation
│   ├── 9.  Basic Forecasting Techniques
│   ├── 10. Simple Exponential Smoothing
│   ├── 11. Holt's Linear Trend Model
│   ├── 12. Holt-Winters Forecasting
│   ├── 13. Residuals
│   ├── 14. Cross Validation
│   ├── 15. Autoregression (AR)
│   ├── 16. Moving Average (MA) Models
│   ├── 17. ARIMA
│   ├── 18. SARIMA
│   └── 19. Fourier Series & Harmonic Regression
│
├── 📂 Implementation/
│   └── Brazilian Logistics Data (Where ARIMA Fails)  ← Real-world case study
│
└── 📂 MSTL Decomposition/
    ├── MSTL using Electricity Dataset  ← Advanced multi-season forecasting
    ├── MSTL Research Paper (PDF)
    └── Prophet Research Paper (PDF)
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
9. **Notebooks 15–16** → Autoregression & Moving Averages (the building blocks of ARIMA)
10. **Notebook 17** → ARIMA — the industry workhorse model
11. **Notebook 18** → SARIMA — ARIMA with seasonal awareness

### 🔴 Advanced
> Ready for real-world complexity

12. **Implementation/** → See what happens when ARIMA breaks on messy logistics data
13. **MSTL/** → Multi-Seasonal decomposition for data with multiple seasonal patterns (e.g., hourly electricity with daily AND weekly cycles)

---

## 🧠 Key Concepts Explained Simply

| Term | What It Means |
|------|--------------|
| **Stationarity** | The data's average and variability don't change over time. Models need this to work well. |
| **Seasonality** | A pattern that repeats at regular intervals — e.g., ice cream sales spike every summer. |
| **Trend** | The long-term direction — going up, going down, or flat. |
| **Autocorrelation** | How much today's value resembles yesterday's. High autocorrelation = very predictable data. |
| **ARIMA** | A powerful statistical model combining past values (AR) and past errors (MA) with differencing (I). |
| **SARIMA** | ARIMA + seasonal patterns built in. |
| **Exponential Smoothing** | Forecasting by giving more weight to recent data than older data. |
| **Decomposition** | Splitting a time series into its trend, seasonal, and random (residual) parts. |
| **MSTL** | A modern technique to handle data with *multiple* seasonal cycles (e.g., hour-of-day + day-of-week). |
| **Residuals** | The difference between what the model predicted and what actually happened. Lower = better model. |

---

## 🛠️ How to Run the Notebooks

### 1. Clone the repository
```bash
git clone https://github.com/Vishnu912py/time_series_forecasting.git
cd time_series_forecasting
```

### 2. Install dependencies
```bash
pip install pandas numpy matplotlib statsmodels scikit-learn jupyter
```

### 3. Launch Jupyter
```bash
jupyter notebook
```

Then open any `.ipynb` file and run cells top to bottom. That's it!

> 💡 **Tip:** Use [Google Colab](https://colab.research.google.com/) if you don't want to install anything locally — just upload the notebooks and run them in your browser for free.

---

## 📊 Datasets Used

| Dataset | Used In | What It Is |
|---------|---------|------------|
| `AirPassengers.csv` | Basic concepts | Monthly airline passengers (1949–1960) — a classic benchmark dataset |
| Brazilian Logistics Data | Implementation | Real freight/logistics time series — shows ARIMA's limitations on complex data |
| Electricity Dataset | MSTL Decomposition | Hourly electricity consumption — demonstrates multi-seasonal patterns |

---

## 🔬 Research Papers Included

Two research papers are included in the `MSTL Decomposition/` folder for those who want to go deeper:

- **MSTL Paper** — The original research on Multi-Seasonal-Trend decomposition using LOESS
- **Prophet Paper** — Facebook's forecasting tool designed for business time series with holidays and missing data

---

## 💡 Who Is This For?

- 🎓 **Students** learning data science or machine learning
- 📊 **Analysts** who work with sales, finance, or operational data
- 🧑‍💻 **Developers** adding forecasting to their applications
- 🤓 **Curious minds** who want to understand how predictions are made

---

## 🙋 FAQ

**Q: Do I need to be a math genius to understand this?**
No. The notebooks focus on intuition and code. The math is there if you want it, but you can follow along without it.

**Q: What's the best model to use?**
It depends on your data. Start with ARIMA for most cases. Use SARIMA if you have clear seasonal patterns. MSTL is great for complex, multi-layered seasonal data (like hourly readings).

**Q: Why does ARIMA "fail" on the Brazilian logistics data?**
Real-world data is messy. The implementation notebook shows a case where the data has multiple overlapping patterns that ARIMA can't handle well — and introduces better approaches.

---

## ⭐ Like This Repo?

Give it a star ⭐ if you found it helpful — it helps others discover it too!

---

*Made with 📚 + ☕ by [Vishnu912py](https://github.com/Vishnu912py)*
