# 🩺 Pneumonia Detection from Chest X-Ray Images

### 🎓 Project — ESPRIT (2024)
**Author:** Inès Bennour  
**Institution:** ESPRIT, Tunisia  
**Year:** 2024  

---

## 🧠 Project Overview

This project focuses on building a **Convolutional Neural Network (CNN)** for the **automatic detection of pneumonia** from chest X-ray images.  
The goal is to assist radiologists in early diagnosis by leveraging **deep learning** and **computer vision**.

---

## 🚀 Objectives

- Design a CNN architecture capable of classifying X-ray images into **Pneumonia** vs **Normal**.
- Enhance model performance through:
  - **Data Augmentation**
  - **Fine-tuning of the ResNet50** pre-trained model.
- Achieve high diagnostic accuracy on real-world medical data.

---

## 🧩 Dataset

- **Dataset Used:** [ChestX-ray Pneumonia Dataset (Kaggle)](https://www.kaggle.com/datasets/paultimothymooney/chest-xray-pneumonia)
- **Classes:**  
  - `PNEUMONIA`  
  - `NORMAL`
- **Dataset Split:**  
  - 70% training  
  - 20% validation  
  - 10% testing  

---

## 🏗️ Model Architecture

### 1️⃣ Baseline CNN
- Custom CNN with convolutional + pooling layers.
- Activation: ReLU  
- Optimizer: Adam  
- Loss: Binary Crossentropy  

### 2️⃣ Fine-Tuned ResNet50
- Pre-trained on **ImageNet**.
- Top layers replaced with custom dense layers.
- Data augmentation applied (rotation, zoom, horizontal flip).
- Fine-tuning performed on last layers for optimal performance.

---

## 📊 Results

| Model                | Accuracy | Precision | Recall | F1-Score |
|----------------------|-----------|------------|--------|-----------|
| Baseline CNN         | 87%       | 85%        | 88%    | 86%       |
| **ResNet50 (Fine-Tuned)** | **94%** | **93%** | **95%** | **94%** |

✅ **Final Model Accuracy: 94%**

---

## 🛠️ Technologies & Tools

- **Python**
- **TensorFlow / Keras**
- **OpenCV**
- **Matplotlib / Seaborn**
- **NumPy / Pandas**
- **Jupyter Notebook**

---
