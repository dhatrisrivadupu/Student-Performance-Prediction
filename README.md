# Student Performance Prediction using Machine Learning

## 📌 Project Overview
This repository contains an end-to-end Machine Learning project that predicts student academic outcomes based on demographic, social, and academic factors. By analyzing key indicators such as study time, past failures, and parental background, the model evaluates and classifies whether a student is likely to pass or fail.

## 📊 Dataset Summary
- **Source:** Portuguese secondary school student achievement dataset (`Maths.csv`).
- **Instances:** 395 student records (after removing duplicates).
- **Features:** 33 features including demographic attributes (`sex`, `age`, `address`), socio-economic factors (`Medu`, `Fedu`, `Mjob`, `Fjob`), academic metrics (`studytime`, `failures`), and performance grades (`G1`, `G2`, `G3`).
- **Target Variable:** Binary classification (`Result`: 1 = Pass, 0 = Fail based on final grade $G3 \ge 10$).

## ⚙️ Workflow & Methodology
1. **Data Cleaning & Preprocessing:** Duplicate removal, standard scaling for numerical features, and one-hot encoding for categorical variables via a Scikit-Learn `ColumnTransformer` pipeline.
2. **Exploratory Data Analysis (EDA):** Visualizing feature distributions, correlations, and performance trends using Seaborn and Matplotlib.
3. **Model Evaluation:** Training and evaluating four standard classification algorithms using stratified test splits:
   - Logistic Regression
   - Decision Tree Classifier
   - K-Nearest Neighbors (KNN)
   - Support Vector Machine (SVM)

## 🏆 Key Results
| Model | Accuracy (%) | Fail Precision | Fail Recall |
| :--- | :---: | :---: | :---: |
| **SVM** | **68.35%** | 0.55 | 0.23 |
| **Logistic Regression** | 65.82% | 0.47 | 0.35 |
| **Decision Tree** | 65.82% | 0.48 | 0.50 |
| **KNN** | 60.76% | 0.31 | 0.15 |

> **Best Model:** Support Vector Classifier (SVM) achieved the highest overall accuracy of **68.35%**.

## 🚀 How to Run
1. Clone the repository:
   ```bash
   git clone [https://github.com/dhatrisrivadupu/Student-Performance-Prediction.git](https://github.com/dhatrisrivadupu/Student-Performance-Prediction.git)
