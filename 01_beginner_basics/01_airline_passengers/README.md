# ✈️ Airline Passengers Forecasting  

Forecasting monthly airline passengers using **Exploratory Data Analysis (EDA)**, **time series decomposition**, and **forecasting models** (Naive, Seasonal Naive, ARIMA).  

---

## 🎯 Goal
- Understand time series patterns (trend + seasonality)  
- Build baseline forecasting models  
- Apply ARIMA for improved forecasting accuracy  
- Compare model performance  

---

## 📊 Dataset
- **Name:** International Airline Passengers Dataset  
- **Period:** Jan 1949 – Dec 1960 (monthly data)  
- **Source:** [AirPassengers dataset](https://raw.githubusercontent.com/jbrownlee/Datasets/master/airline-passengers.csv)  
- **Variables:**  
  - `Month` → datetime index  
  - `Passengers` → number of airline passengers (in thousands)  

---

## 🔎 Workflow
1. **Exploratory Data Analysis (EDA)**  
   - Rolling mean & variance  
   - Seasonal patterns (monthly/yearly)  
2. **Time Series Decomposition**  
   - Multiplicative model → yearly seasonality  
3. **Baseline Forecasts**  
   - Naive (last value forward)  
   - Seasonal Naive (same month previous year)  
4. **ARIMA Model**  
   - Parameters tuned via `auto_arima`  
   - Captures both trend & seasonality  
5. **Evaluation**  
   - Metrics: MAE, RMSE  
   - Model comparison  

---

## 📈 Results
- **Naive Forecast** → High error  
- **Seasonal Naive** → Reasonable, captures yearly pattern  
- **ARIMA** → Best among baselines  
  - Example: **MAE ≈ 14.89, RMSE ≈ 18.53**  

---


