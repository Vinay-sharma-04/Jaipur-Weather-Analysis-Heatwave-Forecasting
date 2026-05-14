# Jaipur Weather Analysis & Heatwave Forecasting

A machine learning project to predict heatwave days and forecast next-day maximum temperature using 10 years of historical weather data for Jaipur (2015–2025).

---

## Overview

- **Heatwave Classification** — predicts whether a day will be a heatwave (temp_max >= 40°C)
- **Temperature Regression** — forecasts next-day maximum temperature

Data source: [Open-Meteo API](https://open-meteo.com/)

---

## Results

| Task | Model | Metric | Score |
|------|-------|--------|-------|
| Heatwave Classification | Random Forest | ROC-AUC | 0.986 |
| Heatwave Classification | Random Forest | F1-score | 0.83 |
| Temperature Forecasting | Linear Regression | R² | 0.946 |
| Temperature Forecasting | Linear Regression | MAE | 1.03°C |

Baseline MAE (mean prediction): 4.69°C

---

## Key Techniques

- Lag features (1, 2, 3-day) and rolling averages (3-day, 5-day)
- Cyclical month encoding (sin/cos) to capture seasonality
- Chronological train/test split to prevent data leakage
- Class-weight balancing for imbalanced heatwave labels
- Decision threshold tuning (0.5 → 0.604) to optimize F1-score
- Seasonal error analysis (month-wise MAE)

---

## Tech Stack

Python, Pandas, NumPy, Scikit-learn, Matplotlib, Joblib

---

## Files

- Model.ipynb              — main notebook
- open-meteo-...csv        — raw weather dataset
- heatwave_model.pkl       — saved classifier
- temp_model.pkl           — saved regressor
- heatwave_threshold.json  — optimal decision threshold

---

## Future Scope

- LSTM-based time series model
- Streamlit dashboard for real-time forecasting
