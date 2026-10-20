# Breast Cancer Detection using Logistic Regression

This project focuses on predicting whether a breast mass is **Malignant (M)** or **Benign (B)** using the Wisconsin Breast Cancer dataset and a Logistic Regression machine learning model.

---

## 📌 Project Overview

Early diagnosis of breast cancer significantly increases the chances of successful treatment. This repository contains an end-to-end Machine Learning pipeline implemented in Python to classify cell tumor samples based on features extracted from digitized images of fine needle aspirates (FNA) of breast masses.

---

## 📁 Dataset Description

The dataset (`breast_cancer.csv`) contains **569 rows** and **33 columns**:

- **`id`**: Unique identifier for each sample.
- **`diagnosis`**: Target variable (`M` = Malignant, `B` = Benign).
- **Features (30 continuous metrics)**: Nuclear characteristics calculated from digitized images, including:
  - Radius, Texture, Perimeter, Area
  - Smoothness, Compactness, Concavity
  - Concave points, Symmetry, Fractal dimension
  - *(Each feature includes `mean`, `standard error (se)`, and `worst` values)*

---

## 🛠️ Data Preprocessing & Workflow

1. **Data Cleaning**:
   - Dropped non-informative columns: `id` and `Unnamed: 32` (contains null values).
2. **Target Encoding**:
   - Encoded the categorical `diagnosis` column (`M`/`B`) into numerical values (`1` for Malignant, `0` for Benign) using `LabelEncoder`.
3. **Train-Test Split**:
   - Split dataset into **80% training** and **20% testing** sets (`train_size=0.8`, `random_state=42`).
4. **Feature Scaling**:
   - Standardized feature distributions using `StandardScaler` to ensure optimal performance for Logistic Regression.
5. **Model Training & Prediction**:
   - Trained a `LogisticRegression` model.
   - Evaluated probability thresholds (adjusted classification threshold to `0.4` for decision making).

---

## 📊 Model Performance

- **Accuracy Score**: ~**98.25%**
- **Confusion Matrix**:
  ```text
  [[70   1]
   [ 1  42]]
