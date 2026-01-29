# 📱 Spam SMS Detection

## 🔗 Project Showcase  

This project was part of my **Codsoft Machine Learning Internship – Task 4: SMS Spam Detection**.  
I have shared my work on LinkedIn for professional visibility:  
[LinkedIn Showcase Post](https://www.linkedin.com/posts/sajna-b-bhandary-226713310_codsoft-machinelearninginternship-smsspamdetection-activity-7422656769975435265-kbVo?utm_source=share&utm_medium=member_desktop&rcm=ACoAAE8gun4BwCSz3Zc5Yua4aZBFSiAFyU1oCpQ)


## 📌 Overview
This project detects whether an SMS message is **spam** or **ham (legitimate)** using machine learning techniques.  
It leverages **TF-IDF vectorization** and a **Logistic Regression model** to classify SMS messages with high accuracy.

---

## 📊 Dataset
- **Dataset Used:** `spam.csv` (SMS Spam Collection Dataset)  
- **Columns:**  
  - `label` → Message category (`ham` or `spam`)  
  - `message` → SMS text content  
- **Preprocessing:**  
  - Converted labels: `ham = 0`, `spam = 1`  
  - Lowercased all messages  
  - Removed unused/unnamed columns if present  

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


