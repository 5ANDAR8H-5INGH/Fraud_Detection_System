# Fraud Detection System using Machine Learning

## Project Overview
With the rapid growth of digital payment systems, financial fraud has become a critical challenge. Fraudulent transactions are rare, complex, and occur in real time, making them difficult to detect using traditional rule-based approaches.

This project presents a **Fraud Detection System** built using **machine learning**, specifically the **XGBoost classifier**, to identify fraudulent transactions from historical financial data with high accuracy and low false-positive rates.

---

## Problem Statement
Financial institutions face significant losses due to fraudulent transactions. The key challenges include:
- Highly imbalanced datasets (very few fraud cases)
- Complex and evolving fraud patterns
- Need for real-time and accurate fraud detection

The goal of this project is to develop a scalable and efficient machine learning model that can automatically detect fraudulent transactions while minimizing false alerts.

---

## Solution Approach
The proposed solution uses supervised machine learning to classify transactions as **fraudulent** or **legitimate** by analyzing transaction behavior and balance patterns.

### Key Steps:
1. Data preprocessing and cleaning
2. Feature engineering
3. Model training using XGBoost
4. Performance evaluation using fraud-specific metrics

---

## Dataset
The dataset consists of historical transaction records with the following key attributes:
- Transaction amount
- Transaction type
- Account balances before and after transactions
- Time-related features

Fraudulent transactions are labeled, allowing supervised learning.

---

## Technologies & Libraries Used
- **Python 3**
- **Google Colab / Jupyter Notebook**
- **Pandas** – data manipulation
- **NumPy** – numerical operations
- **Scikit-learn** – data splitting and evaluation metrics
- **XGBoost** – fraud classification model
- **Matplotlib** – data visualization

---

## Feature Engineering
To improve fraud detection accuracy, additional features were created:
- Balance difference before and after transaction
- Transaction hour
- Transaction type encoding
- Removal of irrelevant identifiers

Outliers were retained as they often represent fraudulent behavior.

---

## Machine Learning Model
- **Algorithm:** XGBoost Classifier
- **Reason for Selection:**
  - Handles class imbalance effectively
  - Captures non-linear relationships
  - High performance on structured financial data

### Training Details:
- Train-Test Split: 80% / 20%
- Hyperparameter tuning performed
- Evaluation Metrics:
  - Precision
  - Recall
  - F1-score
  - AUC-Precision Recall Curve (AUC-PR)

---

## Results
- High recall, ensuring most fraudulent transactions are detected
- Low false-positive rate, reducing unnecessary alerts
- Strong performance on imbalanced data using AUC-PR metric
- Transaction amount and balance differences identified as key fraud indicators

---

## Future Enhancements
- Integration with real-time transaction monitoring systems
- Deployment using cloud platforms (Azure)
- Use of deep learning models (LSTM) for sequential fraud patterns
- Adaptive learning for evolving fraud strategies

---
