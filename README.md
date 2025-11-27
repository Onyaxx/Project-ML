# ✈️ Airline Passenger Satisfaction Prediction

##  Project Overview
This Machine Learning project aims to predict airline passenger satisfaction based on flight characteristics and customer feedback. In a highly competitive industry, identifying dissatisfied customers proactively is a key lever for retention.
We developed an end-to-end pipeline, comparing multiple classification models to select the best-performing solution for deployment.

* **Course:** Machine Learning Project
* **Date:** December 2025
* **Authors:** Daniel ORDUY REY, Yanis NAIT KACI, Antoine PORTEIX
* **Specialization:** Data Science & Artificial Intelligence

---

##  Objectives
1.  **Predict Satisfaction:** Classify passengers as "Satisfied" or "Neutral/Dissatisfied" with high accuracy.
2.  **Identify Key Drivers:** Understand which services (e.g., Wifi, Boarding) influence satisfaction the most.
3.  **Benchmark Models:** Compare linear baselines against advanced ensemble methods.

---

##  Methodology
We implemented a robust **Scikit-Learn Pipeline** including:
* **Preprocessing:**
    * Median imputation for numerical missing values (e.g., delays).
    * StandardScaler for numerical features.
    * OneHotEncoder for categorical variables.
* **Models Tested:**
    * Logistic Regression (Baseline & Optimized with GridSearch).
    * Random Forest (Bagging).
    * Voting Classifier (Soft Voting).
    * **XGBoost (Out of Scope - Advanced).**

---

## 🏆 Key Results
After rigorous testing on the test set (20% split), our findings are:

| Model | Accuracy | ROC AUC | F1-Score |
|-------|----------|---------|----------|
| **XGBoost** | **96.15%** | **0.9942** | **0.9551** |
| Random Forest | 96.03% | 0.9933 | 0.9539 |
| Voting Classifier | 94.48% | 0.9856 | 0.9362 |
| Logistic Regression | 87.66% | 0.9275 | 0.8558 |

✅ **Champion Model:** XGBoost is the most reliable model.\\
✅ **Robustness:** Confirmed by 5-Fold Cross-Validation (96.12% ± 0.20%).\\
✅ **Business Drivers:** "Online Boarding" and "In-flight Wifi" are the top predictors of satisfaction.\\

---

## 🚀 How to Run the Project

### 1. Prerequisites
Ensure you have Python 3.x installed.
Install the required libraries:
```bash
pip install -r requirements.txt
