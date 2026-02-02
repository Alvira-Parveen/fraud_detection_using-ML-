# 💳 Fraud Detection using Machine Learning

An **end-to-end machine learning project** for detecting **fraudulent financial transactions** from **large-scale, highly imbalanced data**.  
The project focuses on **model interpretability**, **robust evaluation**, and **actionable business insights** for real-world fraud prevention.

---

## 📌 Problem Statement

Financial fraud poses significant risks to companies and customers.  
Fraudulent transactions are **rare**, evolve over time, and often involve complex patterns such as:

- Rapid fund transfers  
- Account draining  
- Unusually large transaction amounts  

Traditional rule-based systems struggle to adapt to these patterns, leading to:
- ❌ High false negatives (missed fraud)
- ❌ Increased financial losses
- ❌ Poor customer experience

**Goal:** Build a **data-driven fraud detection system** that accurately identifies fraudulent transactions while minimizing missed fraud cases.

---

## 🚀 Project Overview

This project implements a **machine learning–based fraud detection pipeline** using historical financial transaction data.

### Workflow:
- Data cleaning and preprocessing  
- Handling severe class imbalance  
- Feature selection and multicollinearity analysis  
- Model training and evaluation  
- Extraction of business insights  

Both **statistical rigor** and **business reasoning** are emphasized.

---

## 🎯 Objectives

- Detect fraudulent transactions from highly imbalanced data  
- Build interpretable and performance-driven ML models  
- Identify key behavioral fraud patterns  
- Evaluate models using appropriate metrics beyond accuracy  
- Propose actionable fraud prevention strategies  

---

## 📊 Dataset Description

- Simulated real-world financial transaction dataset  
- **6.3M+ transactions** over a 30-day period  
- Hourly time-step granularity  
- Includes transaction type, amount, account balances, and fraud labels  

### ⚠️ Dataset Usage Note
Due to local hardware constraints, a **representative subset of 1 million transactions** was used.  
The approach is **scalable** to the full dataset.

---

## 🧹 Data Preprocessing

Key preprocessing steps performed:

- ✅ Missing value analysis (no critical missing values found)  
- ✅ Outlier analysis (retained due to fraud relevance)  
- ✅ Categorical encoding of transaction type  
- ✅ Removal of non-informative identifiers  
- ✅ Prevention of data leakage (`isFlaggedFraud` removed)  
- ✅ Multicollinearity analysis on balance-related features  

---

## 🤖 Models Implemented

### 1️⃣ Logistic Regression
- Baseline and interpretable model  
- Class imbalance handled using `class_weight='balanced'`  

### 2️⃣ Random Forest Classifier
- Captures non-linear fraud patterns  
- Robust to multicollinearity  
- Provides feature importance for interpretability  

---

## 📈 Model Evaluation

Accuracy alone is misleading for fraud detection tasks.

### Metrics Used:
- Precision  
- Recall (critical for fraud detection)  
- F1-Score  
- ROC-AUC  
- Confusion Matrix  

These metrics provide a realistic assessment of model performance.

---

## 🔑 Key Fraud Indicators Identified

The most influential predictors of fraud include:

- Large transaction amounts  
- High-risk transaction types (TRANSFER, CASH_OUT)  
- Sudden depletion of origin account balance  
- Unusual increase in destination account balance  

These patterns strongly align with real-world fraud behavior.

---

## 🛡️ Business Insights & Prevention Strategy

### Recommended Actions:
- Real-time monitoring of high-value transactions  
- Velocity checks for rapid balance depletion  
- Step-up authentication for suspicious transfers  
- Periodic model retraining to handle fraud pattern drift  

---

## 🛠️ Tech Stack

- **Python**
- **Pandas, NumPy**
- **Scikit-learn**
- **Matplotlib, Seaborn**
- **Jupyter Notebook**

---

## 📁 Project Structure
fraud-detection-ml/
├── fraud_detection.ipynb
├── README.md
├── requirements.txt

> 🚫 Raw dataset not included due to size constraints.

---

## ▶️ How to Run Locally
pip install -r requirements.txt
jupyter notebook

---

## 🔮 Future Enhancements

- Gradient Boosting / XGBoost models
- Cost-sensitive learning
- Real-time streaming fraud detection
- Automated alert threshold optimization

## 📌 Conclusion

This project demonstrates how machine learning can be applied to detect fraudulent financial transactions from large-scale, highly imbalanced data. By combining strong preprocessing, interpretable models, and business insights, the system provides a solid foundation for real-world fraud prevention.

---

## 👩‍💻 Author

**Name**: ALVIRA PARVEEN  
🔗 [LinkedIn](https://www.linkedin.com/in/alvira-parveen-78022536b)  
🌐 [GitHub](https://github.com/Alvira-Parveen)

