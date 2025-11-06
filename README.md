This project builds on the work I began during my Machine Learning Internship at Proya Technology, where I developed a multi-label image classification model using Google Vertex AI to detect and categorize fruit images.
Building upon that foundation, I designed and implemented a custom Convolutional Neural Network (CNN) in TensorFlow/Keras trained on the Fruits-360 dataset, achieving 96.9% accuracy.
The model incorporates data preprocessing, multi-label encoding, and a custom three-layer CNN architecture optimized with global average pooling and dropout for regularization.
This project demonstrates my ability to take a cloud-automated ML pipeline from an internship setting and independently translate it into a fully reproducible deep learning implementation, complete with visualization, evaluation, and open-source documentation.

## 🚀 Overview
- **Framework:** TensorFlow 2 / Keras  
- **Dataset:** Fruits-360 (Kaggle)  
- **Model:** Custom CNN (3 Conv layers + Global Average Pooling + Dense layers)  
- **Goal:** Multi-label classification of fruit images  
- **Accuracy:** **96.9%** on validation data  

## 🧠 Model Architecture

| Layer (type) | Output Shape | Param # |
|---------------|--------------|---------|
| Conv2D | (None, 98, 98, 32) | 896 |
| MaxPooling2D | (None, 49, 49, 32) | 0 |
| Conv2D | (None, 47, 47, 64) | 18,496 |
| MaxPooling2D | (None, 23, 23, 64) | 0 |
| Conv2D | (None, 21, 21, 128) | 73,856 |
| GlobalAveragePooling2D | (None, 128) | 0 |
| Dense | (None, 256) | 33,024 |
| Dropout | (None, 256) | 0 |
| Dense | (None, 131) | 33,667 |
| **Total params** | **159,939 (624 KB)** | |

---

## 📈 Training Results

**Validation Accuracy:** `0.969`  
**Validation Loss:** `0.18`  
<img width="277" height="435" alt="Loss_Curve" src="https://github.com/user-attachments/assets/4367b2bf-222c-496d-b6bb-bc4d68f3e756" />        <img width="483" height="374" alt="image" src="https://github.com/user-attachments/assets/8d1de08c-f5ee-46c7-86ff-bcbd1e18814f" />




