# Airline Passengers Forecasting 
 
Goal: Forecast monthly airline passengers using EDA, decomposition, baseline models, and ARIMA. 
 
Steps: 
1. Exploratory Data Analysis 
2. Seasonal Decomposition 
3. Baseline Forecasts (Naive, Seasonal Naive) 
4. ARIMA Forecast 
5. Evaluation 

## 📊 Dataset
- **Name:** International Airline Passengers Dataset
- **Period:** Jan 1949 – Dec 1960 (monthly data)
- **Source:** [AirPassengers dataset](https://raw.githubusercontent.com/jbrownlee/Datasets/master/airline-passengers.csv)
- **Variables:** 
  - `Month` → datetime index
  - `Passengers` → number of airline passengers (in thousands)

---

## 🔎 Steps Followed
1. **Exploratory Data Analysis (EDA)**
   - Trend, rolling mean & variance
   - Monthly seasonal patterns
2. **Time Series Decomposition**
   - Multiplicative model → clear yearly seasonality
3. **Baseline Models**
   - Naive (last value carried forward)
   - Seasonal Naive (same month previous year)
4. **ARIMA Model**
   - Selected using `auto_arima`
   - Captures both trend and seasonality
5. **Evaluation**
   - Metrics: MAE, RMSE
   - Compared Naive vs Seasonal Naive vs ARIMA

---

## 📈 Results Summary
- **Naive Forecast** → High error, poor fit
- **Seasonal Naive** → Better, captures yearly pattern
- **ARIMA** → Best model among baselines
  - Example: MAE ≈ *14.89*, RMSE ≈ *18.53* (fill with your notebook results)

👉 See `results_airline_passengers.csv` for final forecasts.
