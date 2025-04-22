# OEE Prediction

This repository contains a Jupyter Notebook that predicts Overall Equipment Effectiveness (OEE) using machine learning, LightGBM model.

## 🔍 Machine Learning Model

After working with LSTM, CNN and a hybrid model of both LSTM and CNN, I got the best results with a **LightGBM Regressor** to predict OEE as a continuous target between 0 and 1. 

### Why LightGBM?
- It handles missing values and categorical variables well
- Fast training time, even with large datasets
- Performs better on this dataset (tested)

### Closer Look to the Data, Features Used in Model:
- **Minute-by-minute timestamp** for each hydraulic machine
- **Machine state** (`1` = working, `0` = stopped)
- **Shift indicators** (working day vs. weekend)

## 🚀 Deployment Preview

Live web interface for OEE prediction, deployed with real-time shift estimates.

![OEE Prediction UI](screenshot oee.png)
