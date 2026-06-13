# 🛡️ Financial Fraud Detection – Advanced Visualization Notebook


![Python](https://img.shields.io/badge/Python-3.10+-blue?style=for-the-badge&logo=python)
![Pandas](https://img.shields.io/badge/Pandas-Data%20Analysis-150458?style=for-the-badge&logo=pandas)
![NumPy](https://img.shields.io/badge/NumPy-Numerical%20Computing-013243?style=for-the-badge&logo=numpy)
![Plotly](https://img.shields.io/badge/Plotly-Interactive%20Visualization-3F4F75?style=for-the-badge&logo=plotly)
![Matplotlib](https://img.shields.io/badge/Matplotlib-Visualization-orange?style=for-the-badge)
![Seaborn](https://img.shields.io/badge/Seaborn-Statistical%20Plots-4C72B0?style=for-the-badge)
![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-F37626?style=for-the-badge&logo=jupyter)
![EDA](https://img.shields.io/badge/EDA-Exploratory%20Data%20Analysis-success?style=for-the-badge)
![Fraud Detection](https://img.shields.io/badge/Fraud-Detection-red?style=for-the-badge)
![Financial Analytics](https://img.shields.io/badge/Financial-Analytics-green?style=for-the-badge)
![Data Science](https://img.shields.io/badge/Data-Science-purple?style=for-the-badge)
![License](https://img.shields.io/badge/License-MIT-yellow?style=for-the-badge)

An end-to-end exploratory data analysis (EDA) and visualization project for financial fraud detection using the Kaggle Financial Fraud Detection Dataset.

This notebook focuses on discovering fraud patterns, analyzing transaction behavior, identifying risk indicators, and creating professional interactive visualizations suitable for machine learning and fraud analytics projects.

---

## 📌 Project Overview

Financial institutions process millions of transactions daily, making fraud detection a critical challenge.

This notebook performs comprehensive visual analysis on over **6.3 million transactions** to identify:

- Fraud trends
- High-risk transaction patterns
- Transaction type behavior
- Time-based fraud activities
- Outliers and anomalies
- Correlation between financial features
- Fraud indicators for future machine learning models

---

![Kaggle Dataset](https://img.shields.io/badge/Kaggle-Dataset-20BEFF?style=for-the-badge&logo=kaggle)
![Feature Engineering](https://img.shields.io/badge/Feature-Engineering-FF6F00?style=for-the-badge)
![Anomaly Detection](https://img.shields.io/badge/Anomaly-Detection-D32F2F?style=for-the-badge)
![Cyber Security](https://img.shields.io/badge/Cyber-Security-000000?style=for-the-badge&logo=securityscorecard)
![Financial Fraud](https://img.shields.io/badge/Financial-Fraud%20Analytics-F43F5E?style=for-the-badge)
![Transactions](https://img.shields.io/badge/6.3M+-Transactions-14B8A6?style=for-the-badge)

## 📊 Dataset

Dataset Source:

https://www.kaggle.com/datasets/sriharshaeedala/financial-fraud-detection-dataset

### Features

| Feature | Description |
|----------|-------------|
| step | Time step of transaction |
| type | Transaction type |
| amount | Transaction amount |
| nameOrig | Sender account |
| oldbalanceOrg | Sender balance before transaction |
| newbalanceOrig | Sender balance after transaction |
| nameDest | Receiver account |
| oldbalanceDest | Receiver balance before transaction |
| newbalanceDest | Receiver balance after transaction |
| isFraud | Fraud label |
| isFlaggedFraud | Rule-based fraud flag |

---

## 🎨 Dashboard Theme

Designed using a cybersecurity-inspired fraud analytics theme.

| Purpose | Color |
|----------|---------|
| Primary Background | #1E293B |
| Secondary Background | #0F1E36 |
| Fraud Alert | #F43F5E |
| Warning | #F9A825 |
| Success | #14B8A6 |
| Text | #FFFFFF |
| Cards | #263549 |

---

## 📈 Visualizations Included

### Dataset Overview

- Dataset Shape
- Data Types
- Missing Values
- Duplicate Records
- Memory Usage

### Fraud Distribution

- Pie Chart
- Donut Chart
- Count Plot
- Class Imbalance Analysis

### Transaction Analysis

- Amount Distribution
- Log Amount Distribution
- KDE Plot
- Box Plot
- Violin Plot

### Transaction Type Analysis

- PAYMENT
- CASH_OUT
- TRANSFER
- DEBIT
- CASH_IN

Visualized using:

- Count Charts
- Fraud Rate Charts
- Average Amount Analysis
- Volume Analysis

### Time-Based Analysis

- Fraud Rate by Hour
- Transaction Volume by Hour
- Day vs Night Fraud Analysis
- Fraud Activity Trends

### Fraud Analysis

- Fraud by Amount Bucket
- Fraud by Transaction Type
- Fraud Concentration Analysis

### Correlation Analysis

- Correlation Heatmap
- Interactive Correlation Matrix
- Pair Plot Analysis

### Outlier Analysis

- IQR Method
- Boxplots
- Z-Score Visualization

### Feature Engineering Analysis

- Risk Score Distribution
- Engineered Feature Correlations
- Fraud Indicator Analysis

### Multi-Dimensional Analysis

- Bubble Charts
- Heatmaps
- 3D Scatter Plots

---

## ⚙️ Feature Engineering

The notebook creates additional fraud-related features:

```python
log_amount
is_high_amount
balance_diff_orig
balance_diff_dest
hour
is_night
transaction_velocity
risk_score
amount_to_balance_ratio
destination_balance_change
```

These engineered features help reveal hidden fraud patterns.

---

## 🔍 Key Findings

### 1. Transaction Type Risk

Fraud occurs primarily in:

- TRANSFER
- CASH_OUT

while PAYMENT and CASH_IN transactions contain minimal fraud activity.

### 2. Time-Based Fraud

Fraud activity spikes significantly during:

- 2 AM – 5 AM

indicating suspicious off-hour behavior.

### 3. High-Value Transactions

The highest fraud concentration appears in:

- Top transaction amount buckets
- Large balance movements

### 4. Account Draining Behavior

Fraudulent transactions often:

- Empty sender accounts
- Transfer unusually large amounts

### 5. Extreme Class Imbalance

Fraud accounts for only:

```text
0.129%
```

of all transactions.

### 6. Rule-Based Detection Failure

The built-in fraud flag:

```text
isFlaggedFraud
```

misses the majority of actual fraud cases.

### 7. Strong Fraud Indicators

Top fraud predictors:

- Transaction Amount
- Balance Difference
- Night Transactions
- Transfer Operations
- High-Risk Scores

---

## 🛠 Technologies Used

### Data Processing

- Python
- Pandas
- NumPy

### Visualization

- Plotly
- Matplotlib
- Seaborn

### Statistical Analysis

- SciPy

### Notebook Environment

- Jupyter Notebook

---

## 🚀 Running the Notebook

### Clone Repository

```bash
git clone https://github.com/someshvermagithub/financial-fraud-detection-ai.git
```

### Install Requirements

```bash
pip install pandas numpy matplotlib seaborn plotly scipy
```

### Launch Notebook

```bash
jupyter notebook
```

Open:

```text
Financial_Fraud_Detection_Visualization.ipynb
```

---

## 📁 Current Project Structure

```text
financial-fraud-detection-ai/
│
├── notebooks/
│   └── Financial_Fraud_Detection_Visualization.ipynb
│
├── data/
│   └── data.csv
│
├── README.md
│
└── requirements.txt
```

---

# 🔮 Future Improvements

Planned upgrades for transforming this notebook into a complete fraud detection platform.

```text
financial-fraud-detection-ai/
│
├── data/
│
├── notebooks/
│   └── Financial_Fraud_Detection.ipynb
│

```

### Planned Enhancements

- Machine Learning Models
  - Logistic Regression
  - Random Forest
  - XGBoost
  - LightGBM
  - CatBoost

- Deep Learning Models
  - Artificial Neural Networks
  - Autoencoders

- SHAP Explainability

- Joblib Model Persistence

- Interactive Streamlit Dashboard

- Real-Time Fraud Prediction

- Risk Scoring Engine

- Fraud Investigation Dashboard

- Model Comparison System

- Fraud Alert System

---

## 👨‍💻 Author

Developed as a Financial Fraud Detection Analytics Project for machine learning, data science, and cybersecurity portfolio development.

---
⭐ If you found this project useful, consider giving it a star.
