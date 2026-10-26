# Titanic Survival Prediction

A machine learning project for predicting Titanic passenger survival using six classification algorithms, Stratified 5-Fold Cross-Validation, and Optuna hyperparameter optimization.

## Overview

This project was developed for the **Operation of Artificial Intelligence Model (인공지능모델운영)** course. It focuses on building and evaluating classification models while reducing overfitting and preventing data leakage.

## Features

- Data preprocessing with a custom `GroupMedianImputer`
- Stratified 5-Fold Cross-Validation
- Hyperparameter optimization using Optuna and `TPESampler`
- Performance evaluation across six classification algorithms
- Model comparison using F1-Score, AUROC, PR-AUC, Precision, Recall, and False Positive Rate

## Project Structure

```text
.
├── Crossvalidation&HyperparamerTuning.ipynb
├── assignment_report.pdf
└── README.md
```

## Model Performance

The models were evaluated using Stratified 5-Fold Cross-Validation.

| Model | F1-Score | AUROC | PR-AUC |
|---|---:|---:|---:|
| KNN | 0.7662 | 0.8751 | 0.8413 |
| Logistic Regression | 0.7767 | 0.8731 | 0.8549 |
| Naive Bayes | 0.7087 | 0.8376 | 0.7654 |
| Decision Tree | 0.7710 | 0.8629 | 0.8102 |
| Random Forest | 0.7853 | 0.8787 | 0.8560 |
| **XGBoost** | **0.7957** | **0.8812** | **0.8619** |

**Best Model:** XGBoost achieved the highest F1-Score (0.7957) and AUROC (0.8812) among the six evaluated models.

## Technologies Used

- Python
- Pandas
- NumPy
- Scikit-learn
- XGBoost
- Optuna

## Report

The complete assignment report, including the methodology and experimental results, is available in [`assignment_report.pdf`](assignment_report.pdf).
