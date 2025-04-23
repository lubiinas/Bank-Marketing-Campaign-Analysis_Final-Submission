# Bank-Marketing-Campaign-Analysis
ML project using Random Forest for classification (term deposit subscription) and regression (balance prediction) on bank marketing data. Includes preprocessing, feature selection, model tuning, and joblib model saving.
# 💼 Bank Marketing Campaign Analysis

This project aims to analyze and model customer behavior based on a direct marketing campaign by a Portuguese bank. Using machine learning techniques, we perform **classification** to predict whether a client will subscribe to a term deposit and **regression** to understand how numerical features (like balance) influence customer behavior.

---

## 🎯 Project Objectives

- **Classification Task:** Predict whether a client will subscribe to a term deposit (Target: `y`)
- **Regression Task:** Predict the customer's `balance` based on other features

---

## 📊 Dataset

- **Source:** UCI Bank Marketing Dataset
- **File Used:** `bank-full.csv` → Preprocessed into `bank-full-processed.csv`
- Contains customer demographics, job, contact info, campaign outcomes, and more

---

## 🧱 Project Structure
Bank-Marketing-Campaign-Analysis/ │ ├── README.md # Project overview ├── bank-full.csv # Original dataset ├── bank-full-processed.csv # Cleaned and preprocessed dataset │ ├── Phase1_Exploration.ipynb # Data loading, cleaning, EDA, outlier detection ├── Phase2_Model_Building.ipynb # Model training (classification & regression) ├── Phase3_Feature_Selection.ipynb # Feature selection and hyperparameter tuning ├── Phase4_Model_Saving.ipynb # Saving final models using joblib │ ├── best_classifier_model.pkl # Saved classification model ├── best_regressor_model.pkl # Saved regression model └── requirements.txt # Python libraries used


---

## 🔬 Project Phases Summary

### 📍 Intermediate + Phase 1 – Data Cleaning & Exploration
- Loaded dataset
- Handled missing values
- Described data statistically
- Detected outliers using boxplots
- Visualized class distribution

### 📍 Phase 2 – Model Building
- Trained a `RandomForestClassifier` to predict term deposit subscription (`y`)
- Trained a `RandomForestRegressor` to predict customer `balance`
- Evaluated with:
  - ✅ Accuracy, classification report (for classifier)
  - 📊 MAE, MSE (for regression)

### 📍 Phase 3 – Feature Selection & Hyperparameter Tuning
- Identified most important features using feature importances
- Tuned hyperparameters using `GridSearchCV`
- Evaluated using:
  - Confusion matrix
  - R² score

### 📍 Phase 4 – Model Saving
- Saved final models using `joblib`:
  - `best_classifier_model.pkl`
  - `best_regressor_model.pkl`
- Models are now ready for deployment/integration

---

## ⚙️ Technologies Used

- Python
- Pandas, NumPy
- Scikit-learn
- Matplotlib, Seaborn
- Jupyter Notebook
- Joblib

---

## 💡 How to Run This Project

1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/Bank-Marketing-Campaign-Analysis.git
   cd Bank-Marketing-Campaign-Analysis



