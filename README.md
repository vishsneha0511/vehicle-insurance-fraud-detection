# 🚗 Vehicle Insurance Fraud Detection using Machine Learning

## 📌 Project Overview

Insurance fraud is a significant challenge for insurance companies, leading to substantial financial losses and increased operational costs. Detecting fraudulent claims manually is time-consuming and often ineffective due to the large volume of claims processed daily.

This project develops an end-to-end Machine Learning pipeline to predict whether a vehicle insurance claim is **fraudulent** or **legitimate** using historical insurance claim data. The workflow includes data preprocessing, handling class imbalance using SMOTE, training multiple classification models, hyperparameter tuning, model evaluation, and feature importance analysis.

---

# 🎯 Business Problem

Insurance companies receive thousands of claims every day, making manual fraud detection inefficient and expensive. An automated fraud detection system can help identify suspicious claims early, enabling faster investigation, reducing financial losses, and improving operational efficiency.

---

# 🎯 Project Objectives

- Build a binary classification model to detect fraudulent insurance claims.
- Perform comprehensive Exploratory Data Analysis (EDA).
- Preprocess the dataset for machine learning.
- Handle severe class imbalance using SMOTE.
- Compare multiple machine learning classification algorithms.
- Optimize the best-performing model using GridSearchCV.
- Evaluate model performance using multiple classification metrics.
- Interpret model predictions using Feature Importance analysis.
- Conduct a feature selection experiment to evaluate model simplification.

---

# 📊 Dataset Information

**Dataset:** Vehicle Insurance Fraud Detection Dataset

**Source:** Kaggle

| Attribute | Value |
|-----------|-------|
| Total Records | 15,420 |
| Total Features | 33 |
| Target Variable | FraudFound_P |
| Fraud Cases | 923 (~6%) |
| Non-Fraud Cases | 14,497 (~94%) |

---

# 🔄 Project Workflow

```text
Business Understanding
        ↓
Dataset Understanding
        ↓
Exploratory Data Analysis (EDA)
        ↓
Data Preprocessing
        ↓
Train-Test Split
        ↓
One-Hot Encoding
        ↓
Feature Scaling
        ↓
SMOTE (Training Data Only)
        ↓
Model Building
        ↓
Model Comparison
        ↓
Hyperparameter Tuning
        ↓
Model Evaluation
        ↓
Feature Importance
        ↓
Feature Selection Experiment
        ↓
Final Conclusion
```

---

# 🛠️ Tech Stack

- Python
- Pandas
- NumPy
- Matplotlib
- Scikit-learn
- XGBoost
- Imbalanced-learn (SMOTE)
- Joblib
- Jupyter Notebook

---

# ⚙️ Machine Learning Pipeline

### 1. Data Preprocessing

- Removed irrelevant identifier columns.
- Applied One-Hot Encoding for categorical variables.
- Applied StandardScaler to numerical features.

### 2. Handling Class Imbalance

- Applied SMOTE only on the training dataset to generate synthetic minority class samples and avoid data leakage.

### 3. Model Building

The following classification algorithms were trained and compared:

- Logistic Regression
- Decision Tree
- Random Forest
- Support Vector Machine (SVM)
- XGBoost

### 4. Hyperparameter Tuning

The best-performing model was optimized using **GridSearchCV** to obtain the optimal hyperparameter combination.

### 5. Model Evaluation

Models were evaluated using:

- Accuracy
- Precision
- Recall
- F1-Score
- ROC-AUC
- Confusion Matrix
- Classification Report

### 6. Model Explainability

- Feature Importance Analysis
- Feature Selection Experiment

---

# 🤖 Models Implemented

| Model | Purpose |
|--------|----------|
| Logistic Regression | Baseline Linear Classifier |
| Decision Tree | Tree-Based Model |
| Random Forest | Ensemble Learning |
| Support Vector Machine | Margin-Based Classifier |
| XGBoost | Gradient Boosting Classifier |

---

# 📈 Performance Metrics

The following evaluation metrics were used to assess model performance:

- Accuracy
- Precision
- Recall
- F1-Score
- ROC-AUC Score

Since fraudulent claims represent only a small proportion of the dataset, Recall and ROC-AUC were considered particularly important during model evaluation.

---

# 🏆 Key Results

- Successfully built an end-to-end fraud detection pipeline.
- Performed comprehensive EDA and preprocessing.
- Addressed severe class imbalance using SMOTE.
- Compared five supervised classification algorithms.
- Optimized the best model using GridSearchCV.
- Evaluated model performance using multiple classification metrics.
- Identified the most influential features affecting fraud prediction.
- Conducted a feature selection experiment to study the effect of reducing the feature space.

---

# 📊 Feature Importance

Feature importance analysis revealed that policy-related and claim-related attributes contributed most to fraud prediction.

Top influential features included:

- BasePolicy
- Fault
- AddressChange_Claim
- PolicyType
- VehiclePrice

---



# 🔮 Future Improvements

- Perform threshold tuning for improved fraud detection.
- Compare SMOTE with ADASYN and Borderline-SMOTE.
- Apply SHAP values for local model explainability.
- Deploy the trained model using Flask or FastAPI.
- Retrain the model with updated insurance claim data.

---

# 👩‍💻 Author

**Sneha Vishwakarma**

M.Sc. Applied Statistics & Informatics

Indian Institute of Technology Bombay (IIT Bombay)

---

## ⭐ If you found this project useful, consider giving it a Star!
