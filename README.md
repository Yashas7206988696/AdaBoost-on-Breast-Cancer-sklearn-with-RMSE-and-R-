# AdaBoost on Breast Cancer - sklearn with RMSE and R²

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/Yashas7206988696/AdaBoost-on-Breast-Cancer-sklearn-with-RMSE-and-R-/blob/main/CODE.ipynb)

## 📋 Project Overview

This repository implements an **AdaBoost Classifier** using scikit-learn to classify breast cancer cases as malignant or benign. The project demonstrates the application of ensemble learning techniques on the Wisconsin Breast Cancer Diagnostic dataset, with evaluation using both traditional classification metrics and regression-style metrics (RMSE and R²) as specifically requested.

## 🎯 AdaBoost Methodology

### What is AdaBoost?
Adaptive Boosting (AdaBoost) is an ensemble learning algorithm that combines multiple weak learners to create a strong classifier. It works by:

1. **Sequential Learning**: Training weak learners sequentially, where each subsequent learner focuses on the mistakes of previous ones
2. **Adaptive Weighting**: Assigning higher weights to misclassified samples in each iteration
3. **Weighted Voting**: Combining predictions from all weak learners using weighted majority voting

### Model Configuration
- **Base Learner**: Decision Tree Classifier with max_leaf_nodes=10 (shallow trees)
- **Number of Estimators**: 200 weak learners
- **Learning Rate**: 0.5 (controls the contribution of each weak learner)
- **Random State**: 42 (for reproducibility)

## 📊 Dataset Details

**Wisconsin Breast Cancer Diagnostic Dataset**
- **Source**: scikit-learn's `load_breast_cancer()` function
- **Samples**: 569 instances
- **Features**: 30 numerical features computed from breast mass images
- **Target**: Binary classification (0: Malignant, 1: Benign)
- **Feature Types**: Real-valued measurements including:
  - Mean, standard error, and worst values for:
    - Radius, texture, perimeter, area, smoothness
    - Compactness, concavity, concave points, symmetry, fractal dimension

## 🚀 Code Features

### Core Functionality
- **Data Loading**: Automatic dataset loading from scikit-learn
- **Data Preprocessing**: Stratified train-test split (80/20)
- **Model Training**: AdaBoost classifier with decision tree base learners
- **Evaluation**: Comprehensive metrics including:
  - **RMSE** (Root Mean Square Error)
  - **R² Score** (Coefficient of Determination)
  - Additional classification metrics for context

### Key Highlights
- ✅ **Stratified Splitting**: Maintains class distribution in train/test sets
- ✅ **Ensemble Learning**: Leverages 200 weak decision tree learners
- ✅ **Reproducible Results**: Fixed random seed for consistent outputs
- ✅ **Regression Metrics**: RMSE and R² computed on binary predictions as requested
- ✅ **Google Colab Ready**: One-click execution in Colab environment

## 📋 Requirements

```python
scikit-learn>=1.0.0
numpy>=1.21.0
pandas>=1.3.0
matplotlib>=3.4.0
```

## 🔧 Quick Start

### Local Environment
1. **Clone the repository**:
   ```bash
   git clone https://github.com/Yashas7206988696/AdaBoost-on-Breast-Cancer-sklearn-with-RMSE-and-R-.git
   cd AdaBoost-on-Breast-Cancer-sklearn-with-RMSE-and-R-
   ```

2. **Install dependencies**:
   ```bash
   pip install scikit-learn numpy pandas matplotlib
   ```

3. **Run the notebook**:
   - Open `CODE.ipynb` in Jupyter Notebook/Lab
   - Execute all cells to see the results

### Google Colab (Recommended)
**🚀 [Open in Google Colab](https://colab.research.google.com/github/Yashas7206988696/AdaBoost-on-Breast-Cancer-sklearn-with-RMSE-and-R-/blob/main/CODE.ipynb)** - Click to run instantly!

## 📈 Expected Results

The AdaBoost classifier typically achieves:
- **High Classification Accuracy**: ~95-98% on the breast cancer dataset
- **RMSE**: Low error values indicating good prediction quality
- **R² Score**: High coefficient values showing good model fit

*Note: RMSE and R² are regression metrics applied to binary classification as specifically requested, though accuracy, precision, recall, and F1-score are more conventional for classification tasks.*

## 📁 Repository Structure

```
AdaBoost-on-Breast-Cancer-sklearn-with-RMSE-and-R-/
├── CODE.ipynb          # Main implementation notebook
├── README.md           # Project documentation
└── .gitignore         # Git ignore file
```

## 🤝 Contributing

Feel free to fork this repository and submit pull requests for improvements or additional features!

## 📄 License

This project is open source and available under the MIT License.

---

**🔗 Quick Links:**
- 📓 [Jupyter Notebook](CODE.ipynb)
- 🚀 [Run in Google Colab](https://colab.research.google.com/github/Yashas7206988696/AdaBoost-on-Breast-Cancer-sklearn-with-RMSE-and-R-/blob/main/CODE.ipynb)
- 📊 [Scikit-learn Documentation](https://scikit-learn.org/stable/modules/ensemble.html#adaboost)
