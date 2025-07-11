# ✈️ Time Series Forecasting on Air Passengers Dataset

This project demonstrates time series analysis and forecasting techniques using the famous Air Passengers dataset. It involves decomposing the time series, making the data stationary, and applying ARIMA and SARIMA models for prediction.

## 📊 Dataset
The dataset contains monthly totals of international airline passengers from 1949 to 1960.

## 🧪 Techniques Used

- **Seasonal Decomposition** using `seasonal_decompose` from `statsmodels`
- **Stationarity Check** using the Augmented Dickey-Fuller (ADF) Test
- **Trend & Seasonality Removal** via:
  - Logarithmic Transformation
  - Rolling Mean and Standard Deviation
- **Modeling**:
  - ARIMA (AutoRegressive Integrated Moving Average)
  - SARIMA (Seasonal ARIMA)

## 📈 Key Steps

1. **Data Decomposition**  
   Used `seasonal_decompose(df)` to visualize trend, seasonality, and residuals.

2. **Stationarity Testing**  
   Checked with ADF Test. Since the data was not stationary, transformations were applied.

3. **Data Transformation**  
   - Log transformation to stabilize variance
   - Rolling mean and standard deviation plotted for visual inspection

4. **Modeling with ARIMA**  
   Parameters (p, d, q) were chosen based on ACF and PACF plots.  
   Trained ARIMA model on stationary data and forecasted future values.

5. **SARIMA Extension**  
   Applied SARIMA to account for seasonal effects in the data.

## 📚 Libraries Used

- `pandas`
- `matplotlib`
- `numpy`
- `statsmodels`

## 🚀 Output

- Forecasted monthly airline passenger numbers
- Plots for decomposed components, rolling statistics, and forecast results

## 📌 Conclusion

This project illustrates the full cycle of time series forecasting: from visualizing trends to ensuring stationarity and applying predictive models. ARIMA and SARIMA provided meaningful forecasts based on past patterns.

---


