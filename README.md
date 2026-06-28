# 💳 Credit Card Default Prediction using Machine Learning

Predicting customer payment defaults using an end-to-end Machine Learning pipeline for credit risk assessment and informed lending decisions.

**Python • Scikit-Learn • Random Forest • XGBoost • LightGBM • SMOTE • Feature Engineering • ROC-AUC**

---

## 📖 Overview

Credit card default prediction is an important problem in the financial sector. Banks and lending institutions need reliable methods to identify customers who are likely to default on future payments.

This project develops a complete machine learning pipeline to predict credit card defaults using customer demographic information, billing history, payment behavior, and repayment status.

The workflow covers:

- Data Cleaning
- Exploratory Data Analysis (EDA)
- Feature Engineering
- Handling Class Imbalance
- Model Training
- Hyperparameter Tuning
- Model Evaluation

The final objective is to help financial institutions identify high-risk customers and improve credit risk management.

---

## 🎯 Problem Statement

Financial institutions face significant losses when customers fail to repay credit card dues. Predicting potential defaulters in advance enables organizations to make informed lending decisions and reduce financial risk.

The goal of this project is to build a machine learning model capable of predicting whether a customer will default on their next credit card payment based on historical customer data.

---

## 🛠️ Methodology

### 1. Data Cleaning

- Handled missing values
- Corrected inconsistent categorical values
- Checked and removed duplicate records
- Performed data preprocessing and validation

### 2. Exploratory Data Analysis (EDA)

Key analyses performed:

- Class distribution analysis
- Default rate analysis
- Correlation analysis
- Credit limit distribution
- Payment behavior trends
- Billing amount patterns
- Demographic analysis

Key findings:

- Repayment history strongly influences default behavior.
- Customers with higher delinquency scores show significantly higher default rates.
- Credit utilization patterns impact repayment risk.

### 3. Feature Engineering

Created several meaningful features to improve model performance:

- Credit Utilization Ratio
- Average Bill Amount
- Average Payment Amount
- Mean Delinquency Score
- Maximum Delinquency
- Delinquent Months Count
- Payment-to-Bill Ratios
- Age-to-Limit Ratio
- Interaction Features

### 4. Handling Class Imbalance

Applied **SMOTE (Synthetic Minority Oversampling Technique)** to improve minority class representation and enhance model learning.

### 5. Model Training

The following models were trained and evaluated:

- Logistic Regression
- Decision Tree
- Random Forest
- XGBoost
- LightGBM

### 6. Hyperparameter Tuning

Used:

- GridSearchCV
- Cross Validation

to optimize model performance and improve generalization.

### 7. Model Evaluation

Evaluation metrics used:

- Accuracy
- Precision
- Recall
- F1 Score
- F2 Score
- ROC-AUC Score

---

## 📊 Results

### 🏆 Best Model: Random Forest

| Metric | Score |
|----------|----------|
| Accuracy | 88.76% |
| Precision | 88.93% |
| Recall | 88.76% |
| F1 Score | 88.75% |
| F2 Score | 88.73% |
| ROC-AUC | 88.78% |

### Best Model Performance

```text
Accuracy      : 0.887598
Precision     : 0.889348
Recall        : 0.887598
F1 Score      : 0.887494
F2 Score      : 0.887322
ROC-AUC Score : 0.887773
```

The Random Forest model achieved the best overall performance among all evaluated models, providing a strong balance between precision, recall, and classification capability.

---

## 📈 Machine Learning Pipeline

```text
Raw Dataset
     │
     ▼
Data Cleaning
     │
     ▼
Exploratory Data Analysis
     │
     ▼
Feature Engineering
     │
     ▼
SMOTE Balancing
     │
     ▼
Train-Test Split
     │
     ▼
Feature Scaling
     │
     ▼
Model Training
     │
     ▼
Hyperparameter Tuning
     │
     ▼
Model Evaluation
     │
     ▼
Prediction
```

---

## 🛠️ Tech Stack

| Category | Technology |
|-----------|-----------|
| Programming Language | Python |
| Environment | Jupyter Notebook |
| Data Processing | Pandas, NumPy |
| Visualization | Matplotlib, Seaborn |
| Machine Learning | Scikit-Learn |
| Imbalanced Learning | SMOTE |
| Ensemble Models | Random Forest, XGBoost, LightGBM |
| Model Selection | GridSearchCV |

---

## 📁 Repository Structure

```text
Credit-Card-Default-Prediction/
│
├── Dataset/
│   ├── processed_data.csv
│   ├── train_dataset_final1.csv
│   └── validate_dataset_final.csv
│
├── notebooks/
│   ├── EDA.ipynb
│   ├── feature-engineering.ipynb
│   └── model-training-tunning-prediction.ipynb
│
├── submission.csv
│
├── README.md
│
└── requirements.txt
```

---

## ▶️ How to Run

### Clone Repository

```bash
git clone https://github.com/yourusername/Credit-Card-Default-Prediction.git

cd Credit-Card-Default-Prediction
```

### Install Dependencies

```bash
pip install -r requirements.txt
```

### Or Install Packages Manually

```bash
pip install pandas numpy matplotlib seaborn scikit-learn imbalanced-learn xgboost lightgbm
```

### Launch Jupyter Notebook

```bash
jupyter notebook
```

Run notebooks in the following order:

1. `EDA.ipynb`
2. `feature-engineering.ipynb`
3. `model-training-tunning-prediction.ipynb`

---

## 🎯 Key Takeaways

- Repayment history is the strongest predictor of default risk.
- Feature engineering significantly improved model performance.
- SMOTE helped address class imbalance effectively.
- Ensemble methods outperformed simpler machine learning models.
- Random Forest achieved the best overall performance.
- The final model can support financial institutions in identifying high-risk customers and reducing default-related losses.

---
