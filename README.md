# 🌬️ Wind Speed Forecasting in Madrid – Time Series Analysis

## 📌 Project Overview

This project performs a time series analysis of **wind speed in Madrid** using historical weather data spanning from **2014 to 2024**, obtained via the **Open-Meteo API**. The goal is to explore temporal trends and seasonality and forecast wind speed for the year **2025** using robust statistical models.

---

## 🎯 Objectives

- Retrieve and process a 10-year weather dataset from the Open-Meteo API.
- Conduct Exploratory Data Analysis (EDA) to uncover patterns and seasonal effects.
- Apply and compare time series models: **ARMA**, **ARIMA**, and **SARIMA**.
- Perform residual diagnostics and statistical validation.
- Generate reliable wind speed forecasts for 2025.

---

## 🛠️ Technologies & Tools Used

| Tool / Library        | Purpose                                      |
|-----------------------|----------------------------------------------|
| `Python`              | Core programming language                    |
| `Pandas`, `NumPy`     | Data processing and numerical operations     |
| `Matplotlib`          | Data visualization                           |
| `statsmodels`         | Time series modeling (ARIMA, SARIMA, etc.)   |
| `openmeteo_requests`  | API data retrieval from Open-Meteo           |
| `requests_cache`      | Caching API responses                        |
| `retry_requests`      | Retrying failed API calls                    |
| `ADF Test`            | Stationarity testing                         |
| `Ljung-Box Test`      | Residual independence check                  |
| `ACF` / `PACF`        | Autocorrelation diagnostics                  |
| `AIC`, `BIC`          | Model evaluation metrics                     |

---

## 🧪 Project Workflow

### 1. Dataset Collection
- Weather data extracted from Open-Meteo API for Madrid (2014–2024).
- Focused features: wind speed, temperature, and daylight duration.
- API access optimized using caching and retry mechanisms.

### 2. Exploratory Data Analysis (EDA)
- Visual inspection of wind speed over time.
- Detection and handling of missing values and outliers.
- Decomposition of time series into trend, seasonality, and residuals (additive & multiplicative).
- Analysis using ACF and PACF to identify autocorrelation and lag effects.

### 3. Stationarity Testing
- Conducted Augmented Dickey-Fuller (ADF) tests to assess stationarity.
- Applied differencing and transformations to stabilize variance and mean.

### 4. Time Series Modeling
- Compared multiple models:
  - **ARMA**: Autoregression and Moving Average.
  - **ARIMA**: Integrated model accounting for non-stationarity.
  - **SARIMA**: Incorporates seasonal components.
- Model selection based on AIC, BIC, residuals, and visual fit.

### 5. Model Evaluation
- Residual diagnostics using Ljung-Box test to assess white noise.
- Visualization of residuals and forecast error.
- Ensured residuals had no autocorrelation.

### 6. Forecasting
- Forecasted wind speed for the year 2025 using the best-fit model.
- Provided confidence intervals to account for prediction uncertainty.

---

## 📈 Results & Insights

- Seasonal ARIMA models produced accurate forecasts aligned with historical patterns.
- Model diagnostics confirmed robustness with residuals exhibiting white noise behavior.
- The methodology can be extended to other locations and weather variables.

---
