# 📱 Spam SMS Detection

## 📌 Overview
This project detects whether an SMS message is **spam** or **ham (legitimate)** using machine learning techniques.  
It leverages **TF-IDF vectorization** and a **Logistic Regression model** to classify SMS messages with high accuracy.

---

## 📊 Dataset
- **Dataset Used:** `spam.csv`  
- **Columns:**  
  - `v1` → Label (`ham` or `spam`)  
  - `v2` → Message text  
- **Preprocessing:**  
  - Renamed columns to `label` and `message`  
  - Converted labels: `ham = 0`, `spam = 1`  
  - Lowercased all messages  

---

## ⚙️ Workflow
1. **Data Preprocessing**
   - Cleaned and normalized text  
   - Converted labels to numeric values  
   - Train-test split (80/20)  

2. **Feature Engineering**
   - Applied **TF-IDF Vectorization** to convert text into numerical features  
   - Removed English stopwords  

3. **Model Training**
   - Logistic Regression (max_iter=1000)  
   - Other models (Naive Bayes, SVM) can be added for comparison  

4. **Evaluation**
   - Classification Report (Precision, Recall, F1-score)  
   - Accuracy Score  
   - Confusion Matrix Visualization  
   - WordClouds for Spam vs Ham messages  
   - Top spam-indicative words identified  

---

## 🧠 Tech Stack
- **Languages:** Python 🐍  
- **Libraries:**  
  - `pandas`, `numpy`  
  - `matplotlib`, `seaborn`  
  - `wordcloud`  
  - `scikit-learn`  

---
