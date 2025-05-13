# ⚡ Energy Forecasting with Weather and Grid Data

This project forecasts electricity demand, market price, and generation source activation using time-series data and machine learning models.

---

## 🎯 Objectives

- Forecast hourly electricity **demand** and **price** (24h ahead)
- Benchmark predictions against TSO (Transmission System Operator) forecasts
- Analyze the impact of **weather**, **time**, and **location** on:
  - Demand
  - Price
  - Generation source mix
- Predict the **next generation source** to be activated when load increases

---

## 📊 Key Features

- 📈 XGBoost models with lag features for time-series learning
- 🧠 SHAP for explainability of key influencing features
- 📉 MAE & RMSE evaluation vs. TSO forecasts
- 🌍 Interactive dashboards using Plotly Express
- ⚡ Generation source classification (multiclass prediction)

---

## 📁 Repository Structure


energy-forecasting/
├── notebooks/
│   └── Energy_Forecasting.ipynb        # Main analysis notebook
├── data/
│   └── README.md                        # Dataset instructions
├── scripts/
│   └── model_training.py (optional)    # Future modular pipeline
├── requirements.txt
└── README.md

---

## 🧪 Datasets

You will need the following CSV files:

- `energy_dataset.csv`
- `weather_features.csv`

Place them in the `data/` folder. If not available, download them from:
[Kaggle Energy Data](https://www.kaggle.com/datasets/nicholasjhana/energy-consumption-generation-prices-and-weather/data)

---

## 📈 Results Snapshot

- ✅ Generation source prediction accuracy: **~79%** (with lag features)
- ⚔️ TSO vs Model MAE: **lower by X%** on demand prediction
- 🔬 Top features: `wind_speed`, `hour`, `total load actual`, `solar`

  ![image](https://github.com/user-attachments/assets/0726e8ba-469d-40f7-b819-7e27cf45bd50)
  ![image](https://github.com/user-attachments/assets/57a3b018-0576-466c-a907-20632f0d8618)
  ![image](https://github.com/user-attachments/assets/380bb96f-86f3-406f-9f48-4968e5c2fb37)
  ![image](https://github.com/user-attachments/assets/3eaf5a9c-9c05-4fd5-9e19-479f4e424630)
  ![image](https://github.com/user-attachments/assets/35476a3e-8a2f-48be-b376-aa362925e383)



