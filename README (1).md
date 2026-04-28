# 🫀 Heart Disease Prediction — 92% AUC-ROC

![Python](https://img.shields.io/badge/Python-3.9%2B-blue?logo=python&logoColor=white)
![Scikit-learn](https://img.shields.io/badge/Scikit--learn-1.x-orange?logo=scikit-learn&logoColor=white)
![XGBoost](https://img.shields.io/badge/XGBoost-Enabled-green)
![License](https://img.shields.io/badge/License-MIT-lightgrey)
![Status](https://img.shields.io/badge/Status-Complete-brightgreen)

> Predicting heart disease early can save lives. This project applies supervised Machine Learning to classify whether a patient has heart disease based on clinical parameters — achieving a peak **AUC-ROC of 0.92**.

---

## 📌 Project Overview

Heart disease remains one of the leading causes of mortality worldwide. Using the **Cleveland Clinic Heart Disease dataset**, this project benchmarks three ML models and identifies the most reliable clinical predictors for early detection.

---

## ✨ Key Features

- 🔍 **Comprehensive EDA** — Deep dive into clinical features: cholesterol levels, chest pain types, max heart rate, and more
- 🤖 **Model Benchmarking** — Head-to-head comparison of Logistic Regression, Random Forest, and XGBoost
- ⚙️ **Hyperparameter Tuning** — GridSearchCV + 5-fold Cross-Validation for optimal and reliable performance
- 📊 **Feature Importance** — Identified the key medical indicators driving predictions
- 📈 **Full Evaluation Suite** — Accuracy, Precision, Recall, F1, and AUC-ROC

---

## 📂 Dataset

| Property | Details |
|---|---|
| **Source** | Kaggle (Cleveland Clinic Foundation) |
| **Entries** | 297 patients |
| **Features** | 14 clinical attributes |
| **Target** | `condition` — `0` Healthy / `1` Heart Disease |

---

## 🧪 Methodology

```
Raw Data → Preprocessing → EDA → Modeling → Tuning → Evaluation
```

1. **Preprocessing** — Categorical encoding + feature scaling with `StandardScaler`
2. **EDA** — Correlation heatmaps, feature distributions, class balance analysis
3. **Modeling** — Three classifiers trained and compared
4. **Optimization** — GridSearchCV with 5-fold CV to prevent overfitting
5. **Evaluation** — Multi-metric comparison across all models

---

## 📊 Results

| Model | Accuracy | AUC-ROC |
|---|---|---|
| ✅ **Logistic Regression** | **~88%** | **0.92** |
| Random Forest | ~85% | 0.90 |
| XGBoost | ~83% | 0.88 |

> **Insight:** Logistic Regression delivered the best balance of interpretability and performance — a critical advantage in clinical decision-support contexts where model explainability matters.

---

## 🏥 Top Clinical Predictors

| Feature | Description |
|---|---|
| `thal` | Thalassemia test result |
| `ca` | Number of major vessels (fluoroscopy) |
| `cp` | Chest pain type |

---

## 🗂️ Project Structure

```
heart-disease-prediction/
│
├── data/
│   └── heart.csv
│
├── notebooks/
│   └── heart_disease_prediction.ipynb
│
├── models/
│   └── best_model.pkl
│
├── requirements.txt
└── README.md
```

---

## 🚀 Getting Started

### 1. Clone the repository
```bash
git clone https://github.com/amrali067/Heart-Disease-Prediction-Using-ML.git
cd Heart-Disease-Prediction-Using-ML
```

### 2. Install dependencies
```bash
pip install -r requirements.txt
```

### 3. Run the notebook
```bash
jupyter notebook notebooks/heart_disease_prediction.ipynb
```

---

## 🛠️ Tech Stack

- **Python 3.9+**
- **Pandas & NumPy** — Data manipulation
- **Matplotlib & Seaborn** — Visualization
- **Scikit-learn** — Logistic Regression, Random Forest, GridSearchCV
- **XGBoost** — Gradient boosting classifier

---

## 👨‍💻 Author

**Eng. Amr Samir**

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-blue?logo=linkedin)](https://www.linkedin.com/in/amr-ali-a6a38b248/)
[![GitHub](https://img.shields.io/badge/GitHub-Follow-black?logo=github)](https://github.com/amrali067)

---

## 📄 License

This project is licensed under the MIT License — feel free to use and build upon it.
