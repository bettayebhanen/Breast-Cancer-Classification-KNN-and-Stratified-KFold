# Breast-Cancer-Classification-KNN-and-Stratified-KFold
Building on the initial KNN model that achieved 96.5% accuracy, this phase focuses on enhancing reliability and robustness using Stratified K-Fold Cross-Validation.

## 📋 Project Overview

While a single train-test split gives a quick performance snapshot, it can sometimes misrepresent how stable a model truly is.
To ensure trustworthy performance, especially in sensitive domains like healthcare, this project implements Stratified K-Fold Cross-Validation — a method that preserves class balance across folds and provides a more accurate estimate of model reliability

## 🎯 Results

**Cross-Validation**:

**Average Accuracy**: 96.48%

**Observation**: Stable and consistent performance across all folds.

**Final Test Evaluation**:

**Accuracy**: 96.49%

**Misclassifications**: Only 4 out of 114 test cases

**Observation**: 99% success rate in detecting malignant cases

## 📊 Dataset

- **Source**: [Breast Cancer Classification Dataset on Kaggle](https://www.kaggle.com/datasets/sahilnbajaj/cancer-classification/code)
- **Samples**: 569 instances
- **Features**: 30 medical features (mean radius, texture, perimeter, area, etc.)
- **Target**: Binary classification (0 = Benign, 1 = Malignant)

## 🛠️ Technical Implementation

### Algorithms & Tools
- **Algorithm**: K-Nearest Neighbors (KNN)
- **Validation**: Stratified K-Fold (k = 5) from scikit-learn
- **Libraries**: scikit-learn, pandas, numpy, matplotlib, seaborn,
- **Preprocessing**: StandardScaler for feature normalization
- **Evaluation**: Accuracy, Precision, Recall, F1-Score, Confusion Matrix

### Model Configuration
- **n_neighbors**: 5
- **Cross-Validation Splits**: 5 (Stratified)
- **Test Split**: 20% hold-out for final evaluation
- **Feature Scaling**: StandardScaler applied to all features

  ## Key Insight
True progress in machine learning isn’t just about achieving high accuracy ...it’s about building models that are reliable, consistent, and reproducible. 
 By validating with Stratified K-Fold, this project ensures trustworthy results for real-world healthcare applications.
  
