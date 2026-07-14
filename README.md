# End-to-End Customer Churn Prediction Pipeline

## Project Overview

This project demonstrates how to build an end-to-end machine learning pipeline using the Scikit-learn Pipeline API to predict customer churn. The pipeline automates data preprocessing, model training, hyperparameter tuning, evaluation, and model export, making it reusable and production-ready.

The project uses the **Telco Customer Churn** dataset from Kaggle.

---

## Objective

Build a reusable machine learning pipeline that:

- Predicts whether a customer will churn.
- Automates data preprocessing using Scikit-learn Pipeline.
- Performs hyperparameter tuning using GridSearchCV.
- Compares multiple machine learning algorithms.
- Selects the best-performing model.
- Exports the final production-ready pipeline using Joblib.

---

## Dataset

**Dataset:** Telco Customer Churn

https://www.kaggle.com/datasets/blastchar/telco-customer-churn

**Target Variable**

```
Churn
```

- Yes = Customer will leave
- No = Customer will stay

---

## Technologies Used

- Python
- Pandas
- NumPy
- Scikit-learn
- Joblib
- Matplotlib
- Seaborn

---

## Machine Learning Workflow

```
Load Dataset
      ↓
Data Cleaning
      ↓
Missing Value Handling
      ↓
Feature Encoding
      ↓
Feature Scaling
      ↓
ColumnTransformer
      ↓
Scikit-learn Pipeline
      ↓
GridSearchCV
      ↓
Model Training
      ↓
Model Evaluation
      ↓
Model Comparison
      ↓
Save Best Model
      ↓
Prediction on New Data
```

---

## Machine Learning Algorithms

Two classification algorithms were implemented and compared.

### 1. Logistic Regression

- Pipeline API
- StandardScaler
- OneHotEncoder
- GridSearchCV

### 2. Random Forest Classifier

- Pipeline API
- OneHotEncoder
- GridSearchCV

After comparing both models, **Logistic Regression** achieved the best overall performance and was selected as the final production-ready model.

---



---

## Features

- End-to-End ML Pipeline
- Data Cleaning
- Missing Value Imputation
- Feature Scaling
- One-Hot Encoding
- ColumnTransformer
- Logistic Regression
- Random Forest Classifier
- Hyperparameter Tuning using GridSearchCV
- Model Comparison
- Model Evaluation
- Export Best Model using Joblib
- Production-Ready Prediction Pipeline

---

## Model Performance

### Logistic Regression

| Metric | Score |
|---------|-------|
| Accuracy | **80.55%** |
| Precision | **0.66** |
| Recall | **0.56** |
| F1-Score | **0.60** |

### Random Forest

| Metric | Score |
|---------|-------|
| Accuracy | **80.0%** |
| Precision | **0.66** |
| Recall | **0.52** |
| F1-Score | **0.58** |

### Final Model Selection

Both Logistic Regression and Random Forest were trained and optimized using GridSearchCV. Based on the evaluation metrics, Logistic Regression achieved higher Accuracy, Recall, and F1-Score for predicting customer churn. Therefore, Logistic Regression was selected as the final model and exported for deployment.

---

## Installation

Clone the repository

```bash
git clone https://github.com/yourusername/End_to_End_Churn_Pipeline.git
```

Move into the project directory

```bash
cd End_to_End_Churn_Pipeline
```

Install dependencies

```bash
pip install -r requirements.txt
```

---

## Run

```bash
python src/train_pipeline.py
```

---

## Saved Model

The best-performing trained pipeline is saved as:

```
models/
└── logistic_pipeline.pkl
```

The exported pipeline includes:

- Data preprocessing
- Missing value handling
- Feature scaling
- One-Hot Encoding
- Logistic Regression model

This allows predictions on new customer data without performing preprocessing manually.

---

## Skills Demonstrated

- Machine Learning Pipeline Construction
- Scikit-learn Pipeline API
- ColumnTransformer
- Data Preprocessing
- Feature Scaling
- One-Hot Encoding
- Logistic Regression
- Random Forest Classification
- Hyperparameter Tuning using GridSearchCV
- Model Evaluation
- Model Comparison
- Joblib Model Export
- Production-Ready Machine Learning

---

## Future Improvements

- XGBoost
- LightGBM
- CatBoost
- SMOTE for class imbalance
- Flask API Deployment
- Docker Containerization

---

## Author

**Anas Ibrahim**

BS Computer Science

University of Central Punjab (UCP)
