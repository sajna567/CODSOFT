# 💳 Credit Card Fraud Detection

## 🔗 Project Showcase  

This project was part of my **Codsoft Machine Learning Internship – Task 2: Credit Card Fraud Detection**.  
I have shared my work on LinkedIn for professional visibility:  
[LinkedIn Showcase Post](https://www.linkedin.com/posts/sajna-b-bhandary-226713310_codsoft-machinelearninginternship-creditcardfrauddetection-activity-7422653991513341952-lGMW?utm_source=share&utm_medium=member_desktop&rcm=ACoAAE8gun4BwCSz3Zc5Yua4aZBFSiAFyU1oCpQ)


## 📌 Overview
This project implements a machine learning pipeline to detect fraudulent credit card transactions.  
It leverages **Logistic Regression, Decision Tree, and Random Forest** models, with Random Forest achieving the best performance.

---

## 📊 Dataset
- **Training Data:** `fraudtrain.csv`  
- **Testing Data:** `fraudtest.csv`
---

## ⚙️ Workflow
1. **Data Preprocessing**
   - Dropped irrelevant columns (`trans_date_trans_time`, `unix_time`, `first`, `last`, etc.)
   - Encoded categorical variables into numerical codes
   - Standardized features using `StandardScaler`

2. **Handling Class Imbalance**
   - Applied **SMOTE** to balance fraud vs legitimate transactions

3. **Model Training**
   - Logistic Regression → Accuracy: **85.30%**
   - Decision Tree → Accuracy: **96.24%**
   - Random Forest → Accuracy: **96.29%** ✅ (Best Model)

4. **Evaluation**
   - Confusion Matrix (Random Forest)
   - Classification Report (Precision, Recall, F1-score)
   - ROC Curve & AUC (~0.96)

5. **Prediction**
   - Final predictions saved to `fraud_predictions.csv`

---

## 🧠 Tech Stack
- **Languages:** Python 🐍  
- **Libraries:**  
  - Data: `pandas`, `numpy`  
  - Visualization: `matplotlib`, `seaborn`  
  - ML Models: `scikit-learn`  
  - Imbalance Handling: `imblearn`  

---



