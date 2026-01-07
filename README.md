# Fraud Detection in Financial Transactions

## 📖 Project Overview
This project focuses on building a machine learning model to proactively detect
fraudulent financial transactions. The goal is to reduce financial losses and
improve fraud prevention using data-driven insights.

The dataset contains over 6 million transaction records and includes both
legitimate and fraudulent transactions.

---

## 🎯 Business Objective
- Detect fraudulent transactions with high recall
- Minimize financial loss due to fraud
- Provide actionable insights for fraud prevention
- Support real-time fraud monitoring systems

---

## 📊 Dataset Description
- Rows: ~6.3 million
- Columns: 10
- Target Variable: 'isFraud' (1 = Fraud, 0 = Non-Fraud)

### Key Features
- Transaction amount
- Transaction type
- Account balance before and after transaction
- Fraud indicator


## 🧹 Data Cleaning & Preprocessing
- Checked for missing values (none significant found)
- Handled outliers using log transformation on transaction amount
- Removed multicollinearity by analyzing correlation among numeric features
- Encoded categorical variables
- Engineered balance-based fraud indicators

---

## 🤖 Machine Learning Model
- Model Used: **XGBoost Classifier**
- Reason:
  - Handles large datasets efficiently
  - Performs well on imbalanced data
  - Captures non-linear fraud patterns

Class imbalance was handled using `scale_pos_weight`.

---

## 📈 Model Evaluation
The model was evaluated using:
- Precision
- Recall (primary metric)
- F1-score
- ROC-AUC score
- ROC Curve

Recall was prioritized to reduce missed fraud cases.

---

## 🔑 Key Fraud Indicators
- High transaction amount
- Sudden balance reduction in sender account
- Abnormal balance increase in destination account
- Certain transaction types

These factors align with real-world fraud behavior.

---

## 🛡️ Fraud Prevention Recommendations
- Real-time transaction monitoring
- Rule + ML hybrid fraud detection
- Multi-factor authentication for high-risk transactions
- Transaction limits and alerts
- Continuous model retraining and monitoring

---

## 📊 Measuring Effectiveness
- Reduction in fraud losses
- Improvement in fraud detection rate
- Stable false positive rate
- A/B testing before and after model deployment
- Monitoring model drift over time

---

## 🛠️ Tools & Technologies
- Python
- Pandas, NumPy
- Matplotlib, Seaborn
- Scikit-learn
- XGBoost
- Google Colab
- GitHub
