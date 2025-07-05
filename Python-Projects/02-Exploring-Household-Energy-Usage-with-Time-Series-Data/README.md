# ⚡ Exploring Household Energy Usage with Time Series Data

This project explores household electricity consumption patterns using the **Global Active Power** variable from a dataset that contains over 2 million minute-level consumptions recorded between 2006 and 2010. The analysis spans from descriptive statistics and time-based visualizations to advanced time series modeling, with the goal of uncovering usage patterns and building accurate energy forecasts.

<table>
  <tr>
    <td><img src="https://github.com/user-attachments/assets/34f91798-2c55-4628-ae57-2cb0833881a2" width="500" height="500"/></td>
    <td><img src="https://github.com/user-attachments/assets/fa322e70-e450-41c8-9613-26aa64bb8166" width="500" height="1000"/></td>
  </tr>
</table>


## 🧹 Data Preparation

- Imported the dataset in chunks for memory efficiency.
- Removed missing values in the target variable.
- Dropped duplicate rows.
- Created a unified `DateTime` column and extracted temporal features:
  - Hour
  - Day of week
  - Month
  - Year
  - Season (Winter, Spring, Summer, Autumn)
  - Time Slot (Night, Morning, Afternoon, Evening)

---

## 📊 Exploratory Analysis

The notebook investigates average energy consumption across different time slices:

- **Hourly**: Peaks in the early morning and especially in the evening (19:00–21:00).
- **Time Slot**: Evening is the most energy-intensive, night the least.
- **Day of the Week**: Highest on weekends (Saturday and Sunday).
- **Monthly**: Peaks in **December**, dips in **August**.
- **Seasonal**: **Winter** shows the highest average consumption.
- **Yearly**: Consumption remains generally stable with expected seasonal peaks.

🔍 A **2D heatmap** (e.g., hour vs. weekday) highlights that **evening hours on weekends** are the periods with the highest energy usage.

---

## ⏱️ Time Series Decomposition

- Resampled the data at multiple frequencies (daily, weekly, monthly, quarterly, yearly) to examine variability across time scales.
- Applied **seasonal decomposition** (additive model) to daily data:
  - **Trend** is relatively stable (suggesting stationarity).
  - **Seasonal** component repeats consistently each year.
  - **Residuals** are random and centered around zero.

---

## 🧪 Time Series Diagnostics

- Performed the **Augmented Dickey-Fuller test** to check stationarity.
- Used **ACF and PACF plots** to analyze autocorrelation and identify optimal lag orders for modeling.

---

## 🔮 Forecasting Models

Three models were implemented and compared:

1. **ARIMA**
   - Used for short-term non-seasonal forecasting.

2. **SARIMA**
   - Included seasonal components to capture yearly cycles.

3. **Prophet**
   - Captures trend and seasonality with minimal tuning.

Each model was trained on a portion of the dataset and tested on a held-out segment.

---

## 📉 Model Diagnostics & Evaluation

For each model:

- Forecasted future values and compared them against actuals.
- Visualized **forecast vs. actual** with **confidence intervals**.
- Assessed **residuals** with plots and statistical tests (e.g., Ljung-Box).
- Calculated key metrics:
  - **MAE** – Mean Absolute Error
  - **RMSE** – Root Mean Squared Error
  - **MAPE** – Mean Absolute Percentage Error

---

## 📊 Final Comparison

- All models performed well, with **SARIMA and Prophet** slightly outperforming ARIMA due to seasonal effects.
- Prophet showed excellent alignment with actuals and robust handling of yearly seasonality.
- The project concludes with a side-by-side **visual and metric-based comparison** of all models.

---

## ✅ Summary of Insights

- Energy use is **highest in the evening**, especially on **weekends** during **winter months**.
- The household exhibits **strong seasonal patterns** with high regularity.
- Time series models, especially **SARIMA** and **Prophet**, can effectively forecast future usage.

