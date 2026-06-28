💳 Credit Card Default Prediction using Machine Learning

Predicting customer payment defaults using an end-to-end Machine Learning pipeline for risk assessment and credit decision support.

Python • Scikit-Learn • Random Forest • XGBoost • LightGBM • Feature Engineering • SMOTE • ROC-AUC

📖 Overview

Credit card defaults represent a major financial risk for banks and lending institutions. This project develops a complete machine learning pipeline to predict whether a customer will default on their credit card payment in the following month.

The workflow includes:

Data Cleaning
Exploratory Data Analysis (EDA)
Feature Engineering
Handling Class Imbalance
Model Training
Hyperparameter Tuning
Model Evaluation

The objective is to identify high-risk customers and support informed lending decisions.

📑 Table of Contents
Overview
Problem Statement
Methodology
Results
Tech Stack
Repository Structure
How to Run
Key Takeaways
🎯 Problem Statement

Financial institutions issue credit cards to millions of customers. Some customers fail to repay their dues, resulting in financial losses.

The goal of this project is to build a machine learning model that can accurately predict whether a customer is likely to default on their next payment based on historical credit behavior, demographic information, billing amounts, and repayment history.

🛠️ Methodology
1️⃣ Data Cleaning
Handled missing values
Removed inconsistencies in categorical variables
Checked for duplicate records
Performed data validation and preprocessing
2️⃣ Exploratory Data Analysis (EDA)

Key insights discovered:

Class imbalance exists between default and non-default customers.
Repayment history is highly correlated with default behavior.
Credit utilization significantly influences risk.
Billing and payment patterns reveal customer repayment tendencies.

Analysis was performed across:

Age
Education
Marital Status
Credit Limit
Bill Amounts
Payment Amounts
3️⃣ Feature Engineering

Created meaningful features to improve predictive performance:

Credit Utilization Ratio
Average Bill Amount
Average Payment Amount
Mean Delinquency Score
Maximum Delinquency
Delinquent Months Count
Payment-to-Bill Ratios
Age-to-Limit Ratio
Interaction Features
4️⃣ Handling Class Imbalance

Applied SMOTE (Synthetic Minority Oversampling Technique) to improve minority class representation and reduce model bias.

5️⃣ Model Training

The following machine learning models were evaluated:

Logistic Regression
Decision Tree
Random Forest
XGBoost
LightGBM

Hyperparameter tuning was performed using:

GridSearchCV
Cross Validation
6️⃣ Evaluation Metrics

Models were evaluated using:

Accuracy
Precision
Recall
F1 Score
F2 Score
ROC-AUC Score
📊 Results
🏆 Best Model: Random Forest
Metric	Score
Accuracy	88.76%
Precision	88.93%
Recall	88.76%
F1 Score	88.75%
F2 Score	88.73%
ROC-AUC	88.78%
Model Performance
Model	Accuracy
Logistic Regression	Evaluated
Decision Tree	Evaluated
Random Forest	⭐ Best
XGBoost	Evaluated
LightGBM	Evaluated

Random Forest achieved the best overall performance, providing a strong balance between precision, recall, and ROC-AUC while maintaining robust generalization.

📈 Machine Learning Pipeline
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
🛠️ Tech Stack
Category	Technology
Language	Python
Environment	Jupyter Notebook
Data Processing	Pandas, NumPy
Visualization	Matplotlib, Seaborn
Machine Learning	Scikit-Learn
Imbalanced Learning	SMOTE
Ensemble Models	Random Forest, XGBoost, LightGBM
Model Selection	GridSearchCV
📁 Repository Structure
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
▶️ How to Run
Clone Repository
git clone https://github.com/yourusername/Credit-Card-Default-Prediction.git

cd Credit-Card-Default-Prediction
Install Dependencies
pip install -r requirements.txt
Launch Jupyter Notebook
jupyter notebook

Run notebooks in the following order:

1. EDA.ipynb
2. feature-engineering.ipynb
3. model-training-tunning-prediction.ipynb
🎯 Key Takeaways
Repayment history is the strongest predictor of default risk.
Feature engineering improved model performance significantly.
SMOTE helped address class imbalance.
Ensemble models outperformed simpler models.
Random Forest achieved the best overall results.
The final model can assist financial institutions in identifying high-risk customers and improving credit risk management.
