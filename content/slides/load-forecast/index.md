---
title: Electric Load Forecasting Enhanced by Weather Factors
summary: A Comparative Study of GRU, LSTM, and XGBoost on Jamali Power System with Weather Data
authors: [Istifa Shania Putri, Dimas Bangun Fiddiansyah, Agus Trisusanto, Didik Notosudjono]
tags: [Electric load forecasting, GRU, LSTM, XGBoost, Time-series]
categories: []
date: "2025-04-30T00:00:00Z"
slides:
  theme: black
  highlight_style: dracula
---

**Istifa Shania Putri, M.Sc.**  
Graduate Student in Informatics, STEI ITB  
**Dimas Bangun Fiddiansyah, Agus Trisusanto**  
Digital Management Division, PLN  
**Prof. Didik Notosudjono** – Pakuan University

---

## Background

- Electric load forecasting is essential for efficient power management, reducing cost and grid instability
- Traditional models (e.g., ARIMA) have limited capacity for nonlinear, temporal patterns
- Machine Learning, especially RNNs, offers higher accuracy with time-series and weather-based data

---

## Research Gap & Purpose

- Lack of direct comparison between GRU, LSTM, and XGBoost under equal conditions
- Goal: Identify the **best model** for load forecasting using **MAPE, R², RMSE, MAE**

---

## Dataset

- **Source**: PLN Jamali (Java-Madura-Bali) region  
- **Period**: Jan–Jul 2024  
- Includes: Load (MW), temperature, humidity, dew point, rainfall  
- Preprocessing: Missing value imputation, normalization, sequence generation

---

## Exploratory Analysis

- Correlation: Temperature (+0.34) strongest with load  
- Other factors (humidity, dew, rain) show weaker influence  
- Decision: Prioritize temperature in feature selection

---

## Models Evaluated

- **GRU**: Simpler RNN with fast convergence  
- **LSTM**: Handles long-term dependencies  
- **XGBoost**: Gradient-boosted trees, less effective for sequences

---

## Experimental Setup

- Data split: Train/Test with 80:20 ratio  
- Sequences generated for GRU/LSTM (window size: 40)  
- Hyperparameter tuning applied across all models

---

## GRU Architecture

- 2 GRU layers with 150 units  
- Dropout: 0.2  
- Epochs: 60  
- Optimizer: Adam  
- Final Dense layer for prediction

---

## LSTM Architecture

- 2 LSTM layers with 50 units  
- Dropout: 0.3  
- Epochs: 100  
- Sequence Length: 40  
- Final Dense layer for regression output

---

## XGBoost Configuration

- Best Params:  
  - n_estimators: 500  
  - max_depth: 5  
  - learning_rate: 0.1  
  - subsample: 0.8  
  - reg_alpha: 0.01, reg_lambda: 0.1

---

## Result Summary

| Model    | R²     | MAPE (%) | RMSE (MW) | MAE (MW) |
|----------|--------|-----------|-------------|------------|
| GRU      | 0.990 | 0.79      | 273.14     | 205.05     |
| LSTM     | 0.989 | 0.85      | 290.84     | 218.58     |
| XGBoost  | 0.589 | 4.76      | 1810.02    | 1152.77    |

---

## Visualization Summary

- GRU tracks actual values very closely, especially in peak-load  
- LSTM follows well but slightly underperforms GRU  
- XGBoost diverges significantly at high variation points

---

## Conclusion

- GRU provides highest accuracy and lowest error  
- LSTM close competitor, more complex  
- XGBoost less suited for sequence tasks  
- RNN-based models are ideal for **time-series + weather** load forecasting

---

## Recommendation

- Use GRU for short-term load forecasting with environmental factors  
- Combine with real-time weather data for improved operational planning  
- Future work: integrate attention mechanisms or transformer-based models

---

## Acknowledgment

- Special thanks to PLN UIP2B Jamali and PLN Head Office (Digital Management Division) for data support.

---

## Thank You 🙏 
