# 🧠 NeuroNest: Smart Detection of Parkinson's Disease Using AI

NeuroNest is a machine learning-based project aimed at early, non-invasive detection of Parkinson's Disease (PD) using voice signal features. It leverages supervised learning models trained on biomedical voice data to classify individuals as Parkinson’s-positive or healthy.

## 🚀 Project Overview

Parkinson’s Disease affects millions globally, and early detection can significantly improve patient outcomes. This project uses AI to analyze vocal features and predict the presence of PD based on subtle variations in speech, such as jitter, shimmer, and other nonlinear dynamics.

## 📊 Dataset

- Source: Publicly available voice dataset
- Total Samples: 1195 voice recordings
- Features: 24 biomedical voice features (Fo, Fhi, jitter, shimmer, RPDE, PPE, etc.)
- Target: `status` (0 = Healthy, 1 = Parkinson's)

## 🔧 Models Implemented

| Model              | Accuracy | AUC    | Notes                                    |
|-------------------|----------|--------|------------------------------------------|
| Logistic Regression | 89.9%    | 0.59   | Low recall for PD class                  |
| Decision Tree      | 96.7%    | 0.971  | High interpretability                    |
| Random Forest      | 98.9%    | 1.00   | Best overall performance                 |
| ANN (Neural Network)| 96.0%    | 1.00   | Strong generalization with regularization|

## 🛠️ Features

- Grid Search-based hyperparameter tuning
- Cross-validation for robustness
- Stratified splitting to handle class imbalance
- Outlier detection (IQR) and standard scaling
- ROC-AUC, PR curve, confusion matrix visualization
- Feature importance ranking
- ANN architecture with dropout, L2 regularization, early stopping
## ☁️ Google Colab Integration

This project was primarily developed and run on [Google Colab](https://colab.research.google.com/):

- ✅ **No setup required** — runs in the cloud  
- 🚀 **GPU acceleration** — used for training the ANN efficiently  
- 🧪 **Interactive environment** — great for testing model changes  
- 📦 **Pre-installed libraries** — includes scikit-learn, pandas, TensorFlow, etc.

## 📈 Evaluation Metrics

- **Accuracy**
- **Precision & Recall**
- **F1-Score**
- **ROC-AUC**
- **Confusion Matrix**
- **Precision-Recall Curve**

## 👨‍⚕️ Real-World Application

This tool demonstrates the potential for AI-assisted voice-based diagnosis in healthcare, especially in early screening and telemedicine environments.



