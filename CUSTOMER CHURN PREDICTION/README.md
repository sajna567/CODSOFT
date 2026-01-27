# 📉 Customer Churn Prediction

## 📌 Overview
This project predicts whether a bank customer is likely to **churn (leave the service)** using machine learning models.  
It applies **Logistic Regression, Random Forest, and Gradient Boosting**, with **Gradient Boosting delivering the best accuracy (~87%)**.

---

## 📊 Dataset
- **Dataset Used:** [Bank Customer Churn Prediction – Kaggle](https://www.kaggle.com/datasets/shantanudhakadd/bank-customer-churn-prediction)  
- **File Name:** `Churn_Modelling.csv`  
- **Rows:** 10,000 customers  
- **Target Variable:** `Exited` (1 = churn, 0 = retained)  
- **Features:**  
  - CreditScore  
  - Geography  
  - Gender  
  - Age  
  - Tenure  
  - Balance  
  - NumOfProducts  
  - HasCrCard  
  - IsActiveMember  
  - EstimatedSalary  

---

## ⚙️ Workflow
1. **Data Preprocessing**
   - Dropped irrelevant columns (`RowNumber`, `CustomerId`, `Surname`)
   - Encoded categorical variables (`Geography`, `Gender`) using `LabelEncoder`
   - Standardized numerical features with `StandardScaler`

2. **Handling Class Imbalance**
   - Applied **SMOTE** to oversample minority class (churned customers)

3. **Model Training**
   - Logistic Regression  
   - Random Forest  
   - Gradient Boosting ✅ (Best Model)

4. **Evaluation**
   - Accuracy, Precision, Recall, F1-score  
   - Confusion Matrix  
   - ROC Curve & AUC  

5. **Prediction**
   - Predict churn for new customers with probability scores

---

## 🧠 Tech Stack
- **Languages:** Python 🐍  
- **Libraries:**  
  - Data: `pandas`, `numpy`  
  - Visualization: `matplotlib`, `seaborn`  
  - ML Models: `scikit-learn`  
  - Imbalance Handling: `imblearn`  

---

