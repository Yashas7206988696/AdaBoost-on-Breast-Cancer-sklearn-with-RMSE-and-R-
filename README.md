# AdaBoost-on-Breast-Cancer-sklearn-with-RMSE-and-r2
## Overview
This repo trains an **AdaBoostClassifier** with shallow **Decision Trees** (up to 10 leaves) on the scikit‑learn Breast Cancer Wisconsin (Diagnostic) dataset. It uses a stratified train/test split and reports **RMSE** and **R²** on the numeric labels (0/1) as requested. Note: RMSE/R² are regression-style metrics; for classification tasks, typical metrics include accuracy, ROC‑AUC, F1.

## What’s inside
- Data: `load_breast_cancer()` (569 rows, 30 numeric features, binary target).
- Model: `AdaBoostClassifier(estimator=DecisionTreeClassifier(max_leaf_nodes=10), n_estimators=200, learning_rate=0.5, random_state=42)`.
- Split: 80/20 stratified.
- Metrics: RMSE and R² computed on hard label predictions.

## Quick start
1. Create an environment and install deps:
2. pip install scikit-learn numpy pandas matplotlib
3. Save the script as `main.py` and run:
python main.py
