# 🧠 Quantum SVM with Qiskit – Breast Cancer Classification

This project implements a **Quantum Support Vector Machine (QSVM)** using [Qiskit](https://qiskit.org/) to classify tumors as malignant or benign using the **Breast Cancer dataset** from scikit-learn.

Quantum SVMs use quantum circuits to compute a kernel matrix, which is then used in a classical SVM to perform classification.

---

## 📊 Dataset

- **Name**: Breast Cancer Wisconsin Diagnostic Dataset
- **Source**: `sklearn.datasets.load_breast_cancer()`
- **Type**: Binary classification (Malignant vs Benign)
- **Features**: 30 numerical attributes

---

## ⚙️ Technologies Used

- [Qiskit](https://qiskit.org/)
- Qiskit Machine Learning module
- Scikit-learn
- Matplotlib
- Jupyter Notebook / Google Colab

---

## 🧪 How It Works

1. Load and normalize the dataset
2. Use `ZZFeatureMap` to map features to quantum circuits
3. Construct a `QuantumKernel` using Qiskit
4. Train a classical `SVC(kernel='precomputed')` on quantum kernel
5. Evaluate classification accuracy

---

## 📈 Results

The quantum SVM achieved **~99% accuracy** on the test set.

---

## ▶️ How to Run (Colab Friendly)

1. Open this notebook in Google Colab  
2. Run the first cell to install dependencies:

```python
!pip install "qiskit[all]" qiskit-machine-learning scikit-learn matplotlib --quiet
