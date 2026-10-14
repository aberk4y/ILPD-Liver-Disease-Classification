# ILPD Liver Disease Classification & Bias Analysis

## Overview

This project investigates machine learning methods for liver disease classification using the Indian Liver Patient Dataset (ILPD) from the UCI Machine Learning Repository.

The study compares seven classification algorithms and evaluates the effects of feature engineering, feature selection, class balancing, dimensionality reduction, and hyperparameter tuning on model performance. It also examines gender-based differences in false negative rates.

## Methods

- Exploratory Data Analysis (EDA)
- Missing-value imputation and outlier analysis using the IQR method
- Feature engineering with four derived clinical features
- Information Gain for feature selection
- SMOTE for class balancing
- StandardScaler and Principal Component Analysis (PCA)
- GridSearchCV with stratified 5-fold cross-validation
- Ablation study and gender-based bias analysis
- Wilcoxon signed-rank test for model comparison

## Machine Learning Models

- Naive Bayes
- K-Nearest Neighbors (KNN)
- Decision Tree
- Random Forest
- Logistic Regression
- Support Vector Machine (SVM)
- Multi-Layer Perceptron (MLP)

## Results

Random Forest achieved the highest test F1-score among the evaluated models.

| Metric | Score |
|---|---:|
| Accuracy | 0.8205 |
| Precision | 0.8605 |
| Recall | 0.8916 |
| F1-score | 0.8757 |
| ROC-AUC | 0.8636 |

The gender-based analysis identified a higher false negative rate for female patients than for male patients. The findings highlight the importance of evaluating model performance across demographic groups.

## Technologies

Python, Pandas, NumPy, scikit-learn, Matplotlib, Seaborn

## Dataset

Indian Liver Patient Dataset (ILPD), available from the UCI Machine Learning Repository:

https://archive.ics.uci.edu/dataset/225/ilpd+indian+liver+patient+dataset

## Project Report

The accompanying report documents the methodology, model comparison, ablation study, and gender-based bias analysis.

## Disclaimer

This project is an academic machine learning study. Its models are not intended for clinical diagnosis or medical decision-making.
