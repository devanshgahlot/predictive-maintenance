# Predictive Maintenance — Machine Failure Classification

**Can we predict machine failure before it happens?**  
This project uses real sensor data to build a classification model that flags machines likely to fail, reducing unplanned downtime in manufacturing environments.

---

## 📌 Project summary

| | |
|---|---|
| **Dataset** | AI4I 2020 Predictive Maintenance Dataset (UCI / Kaggle) |
| **Records** | 10,000 data points |
| **Task** | Binary classification — predict machine failure (yes/no) |
| **Tools** | Python · Pandas · Matplotlib · Seaborn · Scikit-learn |
| **Status** | In progress |

---

## 🗂️ Repository structure

```
predictive-maintenance/
│
├── data/
│   └── ai4i2020.csv                  # Raw dataset
│
├── notebooks/
│   ├── 01_eda.ipynb                  # Exploratory data analysis
│   ├── 02_feature_engineering.ipynb  # Feature creation and selection
│   └── 03_modelling.ipynb            # Model training and evaluation
│
├── README.md
└── requirements.txt
```

---

## 📊 Dataset features

| Feature | Description |
|---|---|
| `Air temperature [K]` | Ambient air temperature |
| `Process temperature [K]` | Process temperature |
| `Rotational speed [rpm]` | Machine rotational speed |
| `Torque [Nm]` | Applied torque |
| `Tool wear [min]` | Tool wear time |
| `Machine failure` | Target variable (0 = no failure, 1 = failure) |

---

## 🔍 Key findings (EDA)

*To be updated as analysis progresses*

- Class imbalance: ~96.5% no-failure, ~3.5% failure
- Tool wear and torque show strongest correlation with failure
- 5 distinct failure modes identified in the data

---

## 🤖 Modelling approach

1. Handle class imbalance (SMOTE / class weights)
2. Baseline: Logistic Regression
3. Improved: Random Forest / Gradient Boosting
4. Evaluation: Precision, Recall, F1, ROC-AUC (recall prioritised — missing a real failure is costly)

---

## ▶️ How to run

```bash
git clone https://github.com/devanshgahlot/predictive-maintenance
cd predictive-maintenance
pip install -r requirements.txt
jupyter notebook notebooks/01_eda.ipynb
```

---

## 📖 Write-up

Full project write-up on LinkedIn: *[link to be added]*

---

## 👤 Author

**Devansh Gahlot** — M.Eng Mechanical Engineering (Leeds) → Data Scientist  
[LinkedIn](https://www.linkedin.com/in/devansh-gahlot-742101179/) · [GitHub](https://github.com/devanshgahlot)
