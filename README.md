# Electricity Demand Forecasting (Time-Series) with XGBoost

## Overview
Forecasts **hourly electricity demand** using historical PJME energy load data and **XGBoost regression**.  
Time-based and lag features capture daily/weekly patterns, enabling accurate short-term predictions.

---

## Key Features
- **Feature Engineering**:  
  - Calendar (hour, day of week, month, etc.)  
  - Weekend & holiday flags  
  - Lag features (24h, 168h) & rolling averages  
- **Model**: XGBoost Regressor with early stopping  
- **Metrics**: RMSE, MAE, MAPE  
- **Visuals**: Full test period, one-week zoom, feature importance

---

## Results
| Metric | Value |
|--------|-------|
| **RMSE** | 1,672.40 MW |
| **MAE** | 1,246.27 MW |
| **MAPE** | 3.90% |

On average, predictions are within ~3.9% of actual demand.

---

## How to Run
1. Download [`PJME_hourly.csv`](https://www.kaggle.com/datasets/robikscube/hourly-energy-consumption)  
2. Open the notebook in Google Colab or locally  
3. Upload CSV when prompted and run all cells

---

## Tech Stack
Python (Pandas, NumPy, Matplotlib), scikit-learn, XGBoost

---

**Author:** Zak Mohamed

