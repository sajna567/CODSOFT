# 🎬 Movie Genre Classification App

## 📌 Overview
This project is a **Streamlit web application** that predicts the **genre of a movie** based on its plot description.  
It uses **Natural Language Processing (NLP)** techniques with **TF-IDF vectorization** and a **Logistic Regression model** to classify movie plots into genres.

---

## 📊 Dataset
- **Training Data:** `train_data.txt`  
- **Testing Data:** `test_data_solution.txt`  
- **Format:** Custom text file separated by `:::`  
- **Columns:**  
  - `id` → Movie ID  
  - `title` → Movie Title  
  - `genre` → Genre(s) (first genre used for training)  
  - `description` → Plot summary  

---

## ⚙️ Workflow
1. **Data Preprocessing**
   - Loaded training data from `train_data.txt`  
   - Dropped missing values  
   - Extracted the **first genre** for each movie  

2. **Feature Engineering**
   - Applied **TF-IDF Vectorization** with max 5000 features  
   - Removed English stopwords  

3. **Model Training**
   - Logistic Regression with `class_weight="balanced"`  
   - Trained on TF-IDF features  

4. **Evaluation**
   - Tested on `test_data_solution.txt`  
   - Achieved **Test Accuracy: ~85%** 🎯  

5. **Deployment**
   - Built a **Streamlit app (`app.py`)** with a custom background and styled UI  
   - User enters a movie plot → App predicts the genre instantly  

---

## 🧠 Tech Stack
- **Languages:** Python 🐍  
- **Libraries:**  
  - `streamlit` (UI)  
  - `scikit-learn` (ML model, TF-IDF)  
  - `pandas`, `numpy` (data handling)  
  - `pickle` (model persistence)  

---

## 🚀 How to Run

# Install dependencies
pip install -r requirements.txt

# Train the model (optional)
python train.py

# Run the Streamlit app
streamlit run app.py
