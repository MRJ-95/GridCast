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

```
energy-forecasting/
├── notebooks/
│   └── Energy_Forecasting.ipynb        # Main analysis notebook
├── data/
│   └── README.md                        # Dataset instructions
├── scripts/
│   └── model_training.py (optional)    # Future modular pipeline
├── requirements.txt
└── README.md
```

---

## 📦 Setup

```bash
pip install -r requirements.txt
```

---

## 🧪 Datasets

You will need the following CSV files:

- `energy_dataset.csv`
- `weather_features.csv`

Place them in the `data/` folder. If not available, download them from:
[Kaggle Energy Data](https://www.kaggle.com/datasets/nicholasjhana/energy-consumption-generation-prices-and-weather/data)

---

## 📈 Results Snapshot

- ✅ Generation source prediction accuracy: **~70%** (with lag features)
- ⚔️ TSO vs Model MAE: **lower by X%** on demand prediction
- 🔬 Top features: `wind_speed`, `hour`, `total load actual`, `solar`

---

## 🤝 Contributions

Pull requests welcome! Feel free to fork and experiment.

---

## 📜 License

MIT License
