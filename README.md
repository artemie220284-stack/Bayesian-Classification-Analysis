# Naive Bayes Classifier with Detailed Probability Analysis

![Python](https://img.shields.io/badge/Python-3.8+-blue)
![Machine Learning](https://img.shields.io/badge/Machine%20Learning-Bayesian-orange)
![License](https://img.shields.io/badge/License-MIT-green)
![Probability](https://img.shields.io/badge/Probabilistic%20Modeling-Interpretable-purple)

A comprehensive implementation of Naive Bayes classifier with transparent probability calculations, feature contribution analysis, and interpretable predictions for agricultural product quality assessment.

## 🍉 Overview

This project implements a Naive Bayes classifier specifically designed for watermelon quality prediction, featuring detailed probability decomposition and transparent decision-making. The system provides not only predictions but also complete mathematical breakdowns showing how each feature contributes to the final classification.

### 🎯 Key Features
- **Complete Probability Calculations**: Prior, likelihood, and posterior probabilities
- **Feature Contribution Analysis**: Visual breakdown of each feature's impact
- **Mixed Data Types**: Handles both discrete (categorical) and continuous (numeric) features
- **Laplace Smoothing**: Robust probability estimation for unseen categories
- **Interpretable Outputs**: Transparent decision-making with mathematical details
- **Watermelon Dataset**: Realistic agricultural quality prediction scenario

### 📊 Sample Prediction Analysis
For a sample watermelon with features: *青绿，蜷缩，浊响，清晰，凹陷，硬滑，密度=0.697，含糖率=0.460*

**Prediction**: 好瓜 (Good Melon) with 99.8% confidence

**Probability Breakdown**:
- **Bad Melon Total Log-Probability**: -9.920
- **Good Melon Total Log-Probability**: -3.826
- **Key Contributing Features**: 密度 (density) +0.674, 含糖率 (sugar content) -0.402

## 🏗️ System Architecture
```
┌─────────────────────────────────────────────┐
│ Input Features │
│ • Discrete: 色泽, 根蒂, 敲声, 纹理, 脐部, 触感 │
│ • Continuous: 密度, 含糖率 │
└─────────────────────┬───────────────────────┘
│
┌─────────────────────▼───────────────────────┐
│ Naive Bayes Classifier │
│ • Prior Probability Estimation │
│ • Conditional Probability Calculation │
│ • Laplace Smoothing │
│ • Gaussian Distribution for Continuous │
└─────────────────────┬───────────────────────┘
│
┌─────────────────────▼───────────────────────┐
│ Probability Decomposition │
│ • Log-probability Calculations │
│ • Feature Contribution Analysis │
│ • Confidence Scoring │
└─────────────────────┬───────────────────────┘
│
┌─────────────────────▼───────────────────────┐
│ Interpretable Output │
│ • Final Prediction │
│ • Probability Distribution │
│ • Feature Impact Visualization │
└─────────────────────────────────────────────┘
```
