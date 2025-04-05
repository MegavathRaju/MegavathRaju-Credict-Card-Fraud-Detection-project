# 💳 Credit Card Fraud Detection using XGBoost

This project is aimed at detecting fraudulent credit card transactions using machine learning. The dataset is highly imbalanced, and advanced techniques like **SMOTE**, **outlier handling**, and **XGBoost** were used to build a robust model.

---

## 📂 Dataset

- **Source:** [Kaggle - Credit Card Fraud Detection](https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud)
- **Size:** 284,807 transactions
- **Fraudulent:** 492 (0.17%)
- The dataset contains features transformed by **PCA** for privacy.

---

## 📌 Problem Statement

Credit card fraud detection is critical to financial institutions. The goal is to detect rare fraudulent transactions accurately while minimizing false positives.

---

## 🔍 Project Pipeline

1. **Data Preprocessing**
   - Handled missing values (if any)
   - Imputed outliers in `Amount` and `Time` using **median**
   - Standardized `Amount` and `Time` features using **StandardScaler**

2. **Class Imbalance Handling**
   - Used **SMOTE (Synthetic Minority Oversampling Technique)** to balance the dataset

3. **Modeling**
   - Applied **XGBoost Classifier** with optimized hyperparameters
   - Also tested **Random Forest**, **Logistic Regression**

4. **Evaluation Metrics**
   - **Precision**
   - **Recall**
   - **Confusion Matrix**
   - **ROC-AUC Score**
   - **PR-AUC Score**

---

## 📊 Results

**Best Model: XGBoostClassifier**

| Metric         | Score        |
|----------------|--------------|
| Precision      | 0.965        |
| Recall         | 0.848        |
| ROC-AUC Score  | 0.978        |
| PR-AUC Score   | 0.873        |

---

## 📈 Visualizations

- Univariate and Bivariate EDA
- Confusion Matrix
- ROC Curve
- Precision-Recall Curve

---

## 🛠️ Technologies Used

- Python
- Pandas, NumPy
- Scikit-learn
- Imbalanced-learn (SMOTE)
- XGBoost
- Matplotlib, Seaborn
