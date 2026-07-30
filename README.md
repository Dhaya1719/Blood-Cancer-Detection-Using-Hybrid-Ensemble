# 🩸 Blood Cancer Detection using Hybrid Ensemble Deep Learning with Explainable AI

An automated blood cancer (Leukemia) detection system using Hybrid Ensemble Deep Learning and Explainable AI (Grad-CAM). The project classifies microscopic blood smear images into **Leukemia** and **Normal** classes by combining multiple CNN models to improve prediction accuracy and reliability.

## 📌 Features

- Blood cancer (Leukemia) classification from blood smear images
- ResNet50, DenseNet121, and InceptionV3 based CNN models
- Ensemble Learning
  - Hard Voting
  - Soft Voting
  - Learnable Ensemble (Meta Model)
- Class imbalance handling using Class Weights
- Explainable AI using Grad-CAM
- Single image prediction pipeline
- Performance evaluation using confusion matrix and classification report

---

## 🏗️ Model Architecture

Input Image
→ Data Preprocessing
→ ResNet50 + DenseNet121 + InceptionV3
→ Ensemble Learning
→ Final Prediction
→ Grad-CAM Visualization

---

## 📂 Dataset

**Dataset:** C-NMC Leukemia Dataset

- Total Images: **10,661**
- Training Images: **8,528**
- Validation Images: **2,133**

Download Dataset:
https://www.kaggle.com/datasets/shafayou/c-nmc-2019-dataset

---

## 🛠️ Tech Stack

- Python
- TensorFlow
- Keras
- NumPy
- Pandas
- OpenCV
- Scikit-learn
- Matplotlib

---

## 📈 Results

| Model | Accuracy |
|--------|----------|
| ResNet50 | 87.06% |
| DenseNet121 | 78.86% |
| InceptionV3 | 91.05% |
| Hard Voting | 92.97% |
| **Soft Voting** | **93.30%** |
| Learnable Ensemble | 92.92% |

---

## 📷 Sample Results

### System Architecture

![Architecture](images/architecture.png)

---

### Grad-CAM Visualization

![GradCAM](images/gradcam.png)

---

### Single Image Prediction

![Prediction](images/prediction.png)

---

## 📁 Project Structure

```
Blood-Cancer-Detection/
│
├── README.md
├── requirements.txt
├── Blood_Cancer_Detection.ipynb
├── models/
├── images/
└── report/
```

---

## 🚀 Installation

```bash
git clone https://github.com/Dhaya1719/Blood-Cancer-Detection-Using-Hybrid-Ensemble

cd Blood-Cancer-Detection

pip install -r requirements.txt
```

---

## ▶️ Usage

Open the notebook and execute all cells.

```bash
jupyter notebook Blood_Cancer_Detection.ipynb
```

---

## 📜 License

This project is developed for educational and research purposes.
