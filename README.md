# Bone Marrow Cell Classification Using CNN

A deep learning project for classifying bone marrow cell types from microscopic images using Convolutional Neural Networks (CNNs). The project includes both **binary classification** (Benign vs Malignant) and **multi-class categorical classification** (8 cell types).

---

## 📌 Overview

Bone marrow examination is essential for diagnosing hematological disorders such as leukemia, lymphoma, and anemia. Manual microscopic analysis is time-consuming and prone to inter-observer variability. This project leverages CNNs to automate bone marrow cell classification, improving diagnostic speed and consistency.

---

## 📂 Dataset

The dataset consists of microscopic images of bone marrow cells categorized into **8 classes**:

| Label | Abbreviation | Cell Type              | Image Count |
|-------|-------------|------------------------|-------------|
| 0     | ART         | Artefact               | 19,630      |
| 1     | BLA         | Blast                  | 11,973      |
| 2     | EBO         | Erythroblast           | 27,395      |
| 3     | LYT         | Lymphocyte             | 26,242      |
| 4     | NGB         | Band Neutrophil        | 9,968       |
| 5     | NGS         | Segmented Neutrophil   | 29,424      |
| 6     | PLM         | Plasma Cell            | 7,629       |
| 7     | PMO         | Promyelocyte           | 11,994      |

**Total Images: ~1,44,255**

---

## 🧠 Models & Results

### 1. Binary Classification (Benign vs Malignant)

| Metric        | Score   |
|---------------|---------|
| **Accuracy**  | 98.56%  |
| **Precision** | 99.75%  |
| **Recall**    | 98.54%  |
| **F1-Score**  | 99.14%  |
| **AUC**       | 99.88%  |

### 2. Multi-Class Classification (8 Cell Types)

| Metric               | Score   |
|----------------------|---------|
| **Accuracy**         | 89.73%  |
| **Macro Precision**  | 87.70%  |
| **Macro Recall**     | 90.51%  |
| **Macro F1-Score**   | 88.65%  |
| **Macro AUC (OVR)**  | 99.27%  |

#### Per-Class Performance

| Cell Type              | Precision | Recall | F1-Score |
|------------------------|-----------|--------|----------|
| Artefact (ART)         | 93.92%    | 85.56% | 89.55%   |
| Blast (BLA)            | 84.80%    | 86.97% | 85.87%   |
| Erythroblast (EBO)     | 96.89%    | 94.01% | 95.43%   |
| Lymphocyte (LYT)       | 90.52%    | 92.20% | 91.36%   |
| Band Neutrophil (NGB)  | 64.58%    | 92.44% | 76.04%   |
| Seg. Neutrophil (NGS)  | 96.26%    | 82.90% | 89.08%   |
| Plasma Cell (PLM)      | 82.37%    | 94.32% | 87.94%   |
| Promyelocyte (PMO)     | 92.23%    | 95.66% | 93.92%   |

---

## 📁 Project Structure

```
Bone Marrow/
├── Binary/
│   ├── bone_marrow_binary_classification.ipynb   # Binary classification notebook
│   └── Final Binary Results/
│       ├── accuracy_loss_curves.png
│       ├── confusion_matrix.png
│       ├── roc_curve.png
│       ├── classification_report.csv
│       ├── classification_report_best_threshold.csv
│       └── test_metrics.csv
├── Categorical/
│   ├── bone_marrow_Catagorical_classification_Gaurav.ipynb  # Multi-class notebook
│   └── Final Results/
│       ├── accuracy_loss_curves_08class.png
│       ├── confusion_matrix_08class.png
│       ├── classification_report_08class.csv
│       ├── class_information_08class.csv
│       └── overall_metrics_08class.csv
├── Ui/
│   └── app.py                                    # UI application
└── dataset Info.xlsx                              # Dataset metadata
```

---

## 🛠️ Tech Stack

- **Language:** Python
- **Deep Learning:** TensorFlow / Keras
- **Model Architecture:** CNN
- **Visualization:** Matplotlib, Seaborn
- **Notebooks:** Jupyter Notebook

---

## 🚀 Getting Started

### Prerequisites

```bash
pip install tensorflow numpy pandas matplotlib seaborn scikit-learn
```

### Run the Notebooks

1. Open `Binary/bone_marrow_binary_classification.ipynb` for binary classification
2. Open `Categorical/bone_marrow_Catagorical_classification_Gaurav.ipynb` for multi-class classification

---

## 📊 Sample Results

### Binary Classification
- **Accuracy & Loss Curves** — Training vs validation performance
- **Confusion Matrix** — True vs predicted labels
- **ROC Curve** — AUC = 99.88%

### Categorical Classification
- **Accuracy & Loss Curves** — Training vs validation across 8 classes
- **Confusion Matrix** — 8×8 class-wise predictions

---

## 📝 License

This project is for academic and research purposes.

---

## 👥 Contributors

- **Himani Gusain** — [GitHub](https://github.com/himanigusain01)
