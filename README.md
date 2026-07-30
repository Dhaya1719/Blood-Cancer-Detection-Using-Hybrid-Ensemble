# 🩸 Blood Cancer Detection using Hybrid Ensemble Deep Learning with Explainable AI

An automated Blood Cancer (Leukemia) detection system that classifies microscopic blood smear images into **Leukemia** and **Normal** using a hybrid ensemble of deep learning models. The project combines **ResNet50, DenseNet121, and InceptionV3** with ensemble learning techniques and **Grad-CAM Explainable AI** to improve prediction accuracy and model interpretability.

---

## 🚀 Features

- Automated Leukemia detection from microscopic blood smear images.
- Deep learning models: **ResNet50, DenseNet121, and InceptionV3**.
- Ensemble learning using:
  - Hard Voting
  - Soft Voting
  - Learnable Ensemble (Meta Model)
- Class imbalance handling using **Class Weights**.
- Explainable AI with **Grad-CAM** for prediction visualization.
- Single image prediction pipeline.
- Performance evaluation using Confusion Matrix and Classification Report.

---

## 🏗️ System Pipeline

```
Input Blood Smear Image
        │
        ▼
Data Preprocessing
        │
        ▼
ResNet50    DenseNet121    InceptionV3
        │         │             │
        └─────────┴─────────────┘
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
- Train-Validation Split: **80:20**

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
- Jupyter Notebook

---

## 📊 Results

| Model | Accuracy |
|-------|----------:|
| ResNet50 | 87.06% |
| DenseNet121 | 78.86% |
| InceptionV3 | 91.05% |
| Hard Voting | 92.97% |
| **Soft Voting** | **93.30%** |
| Learnable Ensemble | 92.92% |

---

## 📦 Pre-trained Models

The trained models are not included in this repository because they exceed GitHub's recommended file size limit.

Download all trained models from Google Drive:

**Google Drive Folder:**  
(https://drive.google.com/drive/folders/1WaGEb9BluaI_N16neXINtcEw3Q6ukBwY?usp=sharing)
After downloading, create a folder named **models** in the project directory and place the downloaded files inside it.

```
models/
├── resnet50.keras
├── densenet121.keras
├── inceptionv3.keras
└── meta_model.keras
```

> **Note:** Keep the model filenames unchanged so the notebook can load them correctly.

---

## 📁 Repository Structure

```
Blood-Cancer-Detection/
│
├── Blood_Cancer_Detection.ipynb
├── README.md
├── requirements.txt
├── .gitignore
├── LICENSE
│
└── report/
    └── Final_Project_Report.pdf
```

---

## ⚙️ Installation

Clone the repository:

```bash
git clone https://github.com/Dhaya1719/Blood-Cancer-Detection-Using-Hybrid-Ensemble.git
```

Navigate to the project directory:

```bash
cd Blood-Cancer-Detection
```

Install the required dependencies:

```bash
pip install -r requirements.txt
```

---

## ▶️ Usage

1. Download the trained models from the Google Drive link above.
2. Create a **models/** folder in the project directory and place all downloaded model files inside it.
3. Open the notebook:

```bash
jupyter notebook Blood_Cancer_Detection.ipynb
```

4. Run all notebook cells sequentially to train, evaluate, or perform single-image prediction.

---

## 🎯 Project Highlights

- Developed a hybrid ensemble framework using **ResNet50, DenseNet121, and InceptionV3** for automated leukemia detection.
- Achieved **93.30% accuracy** using the **Soft Voting Ensemble**, outperforming individual CNN models.
- Integrated **Grad-CAM Explainable AI** to improve model transparency and visualize regions influencing predictions.
- Implemented a **Learnable Ensemble (Meta Model)** for robust and reliable classification.

---

## 📄 Project Report

The complete project report is available in the **report/** directory.

---

## 🤝 Acknowledgements

- C-NMC 2019 Leukemia Dataset
- TensorFlow & Keras
- Scikit-learn
- OpenCV
- Research community for advancements in deep learning and explainable AI.

---

## 📜 License

This project is developed for educational and research purposes.
