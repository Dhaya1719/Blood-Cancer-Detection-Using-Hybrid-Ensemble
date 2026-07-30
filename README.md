# 🩸 Blood Cancer Detection using Hybrid Ensemble Deep Learning with Explainable AI

An automated blood cancer (Leukemia) detection system that classifies microscopic blood smear images into **Leukemia** and **Normal** using a hybrid ensemble of deep learning models. The project combines **ResNet50, DenseNet121, and InceptionV3** with ensemble learning techniques and **Grad-CAM Explainable AI** to improve prediction accuracy and model interpretability.

---

## ✨ Features

- Automated Leukemia detection from blood smear images
- Deep learning models:
  - ResNet50
  - DenseNet121
  - InceptionV3
- Ensemble Learning
  - Hard Voting
  - Soft Voting
  - Learnable Ensemble (Meta Model)
- Class imbalance handling using Class Weights
- Explainable AI using Grad-CAM
- Single image prediction
- Performance evaluation using Classification Report and Confusion Matrix

---

## 🏗️ Model Pipeline

```
Input Blood Smear Image
        │
        ▼
Data Preprocessing
        │
        ▼
ResNet50    DenseNet121    InceptionV3
        │         │            │
        └─────────┴────────────┘
                  │
          Ensemble Learning
     (Hard Voting | Soft Voting |
       Learnable Ensemble)
                  │
                  ▼
         Final Prediction
        (Leukemia / Normal)
                  │
                  ▼
      Grad-CAM Visualization
```

---

## 📂 Dataset

**Dataset:** C-NMC Leukemia Dataset

- Total Images: **10,661**
- Training Images: **8,528**
- Validation Images: **2,133**
- Training Split: **80%**
- Validation Split: **20%**

Dataset Link:

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

## 📊 Results

| Model | Accuracy |
|--------|---------:|
| ResNet50 | 87.06% |
| DenseNet121 | 78.86% |
| InceptionV3 | 91.05% |
| Hard Voting | 92.97% |
| **Soft Voting** | **93.30%** |
| Learnable Ensemble | 92.92% |

---

## 📦 Pre-trained Models

The trained models are not included in this repository due to GitHub file size limitations.

Download all trained models from Google Drive:

**Google Drive:**  
YOUR_DRIVE_FOLDER_LINK

After downloading, place the files inside the `models/` folder.

```
models/
├── resnet50.keras
├── densenet121.keras
├── inceptionv3.keras
└── meta_model.keras
```

---

## 📁 Project Structure

```
Blood-Cancer-Detection/
│
├── README.md
├── requirements.txt
├── .gitignore
├── LICENSE
│
├── blood-cancer-iden (3).ipynb
│
├── models/
│
└── report/
    └── Final_Project_Report.pdf
```

---

## 🚀 Installation

Clone the repository:

```bash
git clone https://github.com/Dhaya1719/Blood-Cancer-Detection-Using-Hybrid-Ensemble.git
```

Move into the project directory:

```bash
cd Blood-Cancer-Detection
```

Install the required dependencies:

```bash
pip install -r requirements.txt
```

---

## ▶️ Usage

Launch Jupyter Notebook:

```bash
jupyter notebook Blood_Cancer_Detection.ipynb
```

Run all notebook cells sequentially.

> **Note:** Download the trained models from the Google Drive link above and place them inside the `models/` folder before running inference.

---

## 🎯 Project Highlights

- Built a hybrid ensemble framework using **ResNet50, DenseNet121, and InceptionV3**.
- Achieved **93.30% accuracy** using the **Soft Voting Ensemble**.
- Integrated **Grad-CAM Explainable AI** for visual interpretation of predictions.
- Implemented a **Learnable Ensemble (Meta Model)** to improve classification reliability.

---

## 📜 License

This project is intended for educational and research purposes.
