# Electricity-Load-Prediction
## Objective
Forecast next day's electricity load using forecasted weather data, simulating real-world constraints (prediction made at 8:00 AM for the following day).

---

## Contents
- `ElectricityLoadPrediction.ipynb` – Full code: data prep, feature engineering, model training, rolling forecast, SHAP explainability

---

## Highlights
- **Tuned XGBoost (Test Set)**:  
  - MAE: 13.77 MW  
  - RMSE: 17.26 MW  
  - MAPE: 4.55%

- **Rolling Forecast (Simulated Daily at 8 AM)**:  
  - MAE: 24.82 MW  
  - RMSE: 30.06 MW  
  - MAPE: 11.10%

- **Key Contributions**:
  - Time-based feature engineering and lagging
  - GridSearchCV for hyperparameter tuning
  - TimeSeriesSplit cross-validation
  - Realistic rolling forecast simulation
  - SHAP analysis for model explainability

---

## Final Recommendation
Deploy the tuned XGBoost model in a daily pipeline that uses updated forecasted weather data at 8:00 AM to predict the next day’s load. Monitor for seasonal drift and retrain periodically.

---

## Author
Kavya Bhojani  
April 2025

