 # ✍️ Handwritten Text Generation
 
 ## 🔗 Project Showcase  

This project was part of my **Codsoft Machine Learning Internship – Task 5: Handwritten Text Generation**.  
I have shared my work on LinkedIn for professional visibility:  
[LinkedIn Showcase Post](https://www.linkedin.com/posts/sajna-b-bhandary-226713310_codsoft-machinelearninginternship-handwrittentextgeneration-activity-7422657870137188352-X0EV?utm_source=share&utm_medium=member_desktop&rcm=ACoAAE8gun4BwCSz3Zc5Yua4aZBFSiAFyU1oCpQ)

## 📌 Overview
This project demonstrates generating **handwritten-style text** using deep learning.  
It leverages the **IAM Handwriting Dataset** and trains a **Recurrent Neural Network (RNN with LSTM)** to learn character-level sequences and generate realistic handwritten text outputs.

---

## 📊 Dataset
- **Dataset Used:** [IAM Handwriting Dataset (Teklia/IAM-line)](https://huggingface.co/datasets/Teklia/IAM-line)  
- **Splits:**  
  - Train: 6,482 samples  
  - Validation: 976 samples  
  - Test: 2,915 samples  
- **Features:**  
  - `image` → Handwritten text image  
  - `text` → Corresponding transcription  

---

## ⚙️ Workflow
1. **Data Loading**
   - HuggingFace `datasets` library used to load IAM dataset  
   - Images and text pairs extracted  

2. **Preprocessing**
   - Character-level tokenization  
   - Sequence padding  
   - One-hot encoding of labels  

3. **Model Architecture**
   - Embedding Layer (128 dimensions)  
   - LSTM Layer (256 units)  
   - Dense Output Layer with Softmax activation  

4. **Training**
   - Optimizer: Adam  
   - Loss: Categorical Crossentropy  
   - Epochs: 20  
   - Batch Size: 128  

---

## 🧠 Tech Stack
- **Languages:** Python 🐍  
- **Libraries:**  
  - `TensorFlow / Keras`  
  - `HuggingFace Datasets`  
  - `Matplotlib`, `NumPy`  
  - `PIL` (for rendering handwritten text images)  

---


