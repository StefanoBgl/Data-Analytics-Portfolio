# ⚡ Exploring Household Energy Usage with Time Series Data

This project explores household electricity consumption patterns using the **Global Active Power** variable from a dataset that contains over 2 million minute-level consumptions recorded between 2006 and 2010. The analysis spans from descriptive statistics and time-based visualizations to advanced time series modeling, with the goal of uncovering usage patterns and building accurate energy forecasts.



<table>
  <tr>
    <td><img src="https://github.com/user-attachments/assets/8ec7e5a0-d7fa-4ea2-801b-3397ce93ab60" width="650" height="500"/></td>
    <td><img src="https://github.com/user-attachments/assets/d5261acb-c8b3-4f59-9a7f-1e78ddbb6364" width="500" height="500"/></td>
  </tr>
</table>

## 🛠️ Technologies
- pandas
- numpy
- matplotlib
- seaborn
- seasonal_decompose
- adfuller
- plot_acf, plot_pacf
- ARIMA, SARIMAX
- acorr_ljungbox, het_arch, jarque_bera
- Prophet
- mean_absolute_error, mean_squared_error, mean_absolute_percentage_error

## 📈 Insights & Results
- **Prophet** forecasts future consumption effectively well, while **ARMA** and **SARIMA** show their best performance mainly on train data.
- The household consumption exhibits **strong seasonal patterns** with high regularity.
- Energy usage is highest in the **evening**, especially on **weekends** during **winter** months.

## 🧱 Workflow Overview
### 1. Data Preparation

- Imported the dataset in chunks for memory efficiency.
- Removed missing values in the target variable.
- Dropped duplicate rows.
- Created a `DateTime` column and extracted temporal features:
  - Hour
  - Day of week
  - Month
  - Year
  - Season (Winter, Spring, Summer, Autumn)
  - Time Slot (Night, Morning, Afternoon, Evening)

### 2. Exploratory Analysis

The notebook investigates average energy consumption across different time slices:

- **Hourly**: Peaks in the early morning and especially in the evening (19:00–21:00).
- **Time Slot**: Evening is the most energy-intensive, night the least.
- **Day of the Week**: Highest on weekends (Saturday and Sunday).
- **Monthly**: Peaks in **December**, dips in **August**.
- **Seasonal**: **Winter** shows the highest average consumption.
- **Yearly**: Consumption remains generally stable with expected seasonal peaks.

A **2D heatmap** investigates the average consumption across multiple time-dimension: **Hour/Day of week**, **Year/Month**, **Time slot/Day of Week**.


### 3. Time Series Decomposition

- Resampled the data at multiple frequencies (daily, weekly, monthly, quarterly, yearly) to examine variability across time scales.
- Applied **seasonal decomposition** (additive model) to daily data:
  - **Trend** is relatively stable (suggesting stationarity).
  - **Seasonal** component repeats consistently each year.
  - **Residuals** are random and centered around zero.

### 4. Time Series Diagnostics

- Performed the **Augmented Dickey-Fuller test** to check stationarity.
- Used **ACF and PACF plots** to analyze autocorrelation and identify optimal lag orders for modeling.

### 5. Forecasting Models

Three models were implemented and compared:

1. **ARMA** for non-seasonal forecasting.

2. **SARIMA** to include a seasonal component in the forecast.

3. **Prophet** to include multiple seasonal components in the forecast.

Each model was trained on a portion of the dataset and tested on a held-out segment.

### 6. Model Diagnostics & Evaluation

For each model:

- Forecasted future values and compared them against actuals.
- Visualized **forecast vs. actual** with **confidence intervals**.
- Assessed **residuals** with plots and statistical tests (e.g., Ljung-Box).
- Calculated key metrics:
  - **MAE** – Mean Absolute Error
  - **RMSE** – Root Mean Squared Error
  - **MAPE** – Mean Absolute Percentage Error


### 7. Final Comparison

- All models delivered similar performance on train data, while on test the **Prophet** significantly overperformed the other models.
- Prophet forecast is highly responsive to different seasonalities and adapt better to higher variability.
- **SARIMA** and **ARMA** performed much worse on test data, resulting in more uncertainty and less precise forecast.
- The project concludes with a side-by-side **visual and metric-based comparison** of all models.

## 📬 Contact
Feel free to connect with me on [Linkedin](https://www.linkedin.com/in/stefano-baglio/) or reach out via email at s.baglio.personal@outlook.com.


## 🗂️ Folder Structure

```bash
📁 supermarket-sales-analysis/
│
├── 📓 Exploring_Household_Energy_Usage_with_Time_Series_Data.ipynb
├── 📄 README.md
└── 📁 Data/
