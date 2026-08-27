# Credit Card Fraud Detection Using Machine Learning

## Project Overview

This project develops a machine learning-based system to detect potentially fraudulent credit card transactions.

The project uses transaction information such as transaction amount, transaction time, merchant category, foreign transaction status, location mismatch, device trust score, transaction velocity, and cardholder age to classify transactions as fraudulent or non-fraudulent.

## Dataset

The dataset contains 10,000 transaction records.

### Features

- Transaction ID
- Transaction Amount
- Transaction Hour
- Merchant Category
- Foreign Transaction
- Location Mismatch
- Device Trust Score
- Velocity in Last 24 Hours
- Cardholder Age

### Target

- `is_fraud`
  - `0` = Not Fraud
  - `1` = Fraud

## Technologies Used

- Python
- Pandas
- NumPy
- Scikit-learn
- Matplotlib
- Jupyter Notebook

## Machine Learning Models

Two classification algorithms were evaluated:

1. Logistic Regression
2. Random Forest

## Results

| Model | Accuracy | Precision | Recall | F1-Score |
|---|---:|---:|---:|---:|
| Logistic Regression | 99.2% | 81.8% | 60.0% | 69.2% |
| Random Forest | 99.2% | 100.0% | 46.7% | 63.6% |

Logistic Regression was selected as the final model because it achieved higher recall and F1-score for fraud detection.

## Prediction

The final model was tested on a new suspicious transaction and classified it as fraudulent with a predicted fraud probability of 100%.

## Project Structure

```text
Fraud_Detection_Project/
│
├── Fraud_Detection_Project.ipynb
├── credit_card_fraud_10k.csv
├── fraud_detection_model.pkl
├── fraud_detection_scaler.pkl
└── README.md
