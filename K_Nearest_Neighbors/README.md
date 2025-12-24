# Breast Cancer Classification using K-Nearest Neighbors (KNN)

## Overview
This project demonstrates the implementation of the **K-Nearest Neighbors (KNN)** algorithm for a **binary classification** problem using the **Breast Cancer Wisconsin Dataset**.  
The objective is to classify tumors as **Malignant (M)** or **Benign (B)** based on multiple medical features.

---

## Dataset
- **Dataset Name:** Breast Cancer Wisconsin Dataset  
- **Source:** Kaggle  
- **Link:** https://www.kaggle.com/datasets/uciml/breast-cancer-wisconsin-data

### Dataset Description
- **Total Rows:** 569  
- **Total Columns:** 33  
  - **Input Features:** 32  
  - **Target Variable:** `diagnosis`  
    - `M` → Malignant  
    - `B` → Benign

---

## Data Preprocessing
- Removed irrelevant columns:
  - `id`
  - `Unnamed: 32`
- Scaled all input features using **StandardScaler** to normalize the data and improve distance-based learning.

---

## Model Workflow
1. Performed data preprocessing and feature scaling.
2. Initialized the KNN classifier with `n_neighbors = 5`.
3. Trained and evaluated the model.
4. Achieved an **accuracy of 97.36%** for `k = 5`.

---

## Hyperparameter Tuning
To determine the optimal number of neighbors, the model was tested with values of `k` ranging from **1 to 15**.

### Results
- **Best Accuracy:** **99.12%**
- **Optimal Value of k:** `n_neighbors = 3`

---

## Technologies Used
- Python  
- NumPy  
- Pandas  
- Scikit-learn  
- Matplotlib / Seaborn

---

## Conclusion
The KNN classifier performed exceptionally well on the Breast Cancer dataset. Proper feature scaling and tuning of the number of neighbors significantly improved model performance, with the highest accuracy achieved at `k = 3`.

---

⭐ If you find this project helpful, consider giving it a star!

