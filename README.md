🛡️ Detecting Insider Threats through Behavioral AI

This repository contains the code, dataset, and machine learning workflow used in a dissertation project on insider threat detection using behavioral data.

🔍 Project Overview

This study evaluates how machine learning (ML) and behavioral AI models can be applied to detect insider threats within corporate environments. Using a simulated organizational dataset (12,000 records), the project develops and compares several ML and deep learning models.

The research also discusses ethical considerations of surveillance analytics, highlighting issues such as fairness, privacy, transparency, and responsible AI deployment.

🧠 Models Implemented

The modelling notebook includes the following algorithms:

Traditional ML Models

Logistic Regression

Random Forest

Support Vector Machine (SVM – RBF Kernel)

XGBoost Gradient Boosting

Deep Learning Model

- Fully Connected Neural Network (TensorFlow/Keras)

Each model is evaluated on:

Accuracy

Precision

Recall

F1-score

ROC-AUC

Confusion Matrix


🗂️ Repository Structure
📁 Detecting-Insider-Threats-through-Behavioral-AI_Dissertation/
│
├── Ver2_Insiderthreat_withgithub.ipynb   # Main modelling notebook
├── insider_logreg_baseline.pkl           # Saved Logistic Regression model
├── insider_random_forest.pkl             # Saved Random Forest model
├── README.md                             # Project documentation
│
└── (More files will be added gradually)


📊 Dataset

A cleaned dataset (AppliedResearchDataset_cleanVer1.csv) was used with:

12,000 rows

15 original attributes (after removing leakage fields)

Balanced classes (6000 insiders, 6000 non-insiders)

Data leakage removal:

event_src (system source bias)

date (temporal leakage pattern)

These fields were removed before modelling.


📌 Future Improvements

Hyperparameter tuning

Explainable AI (SHAP)

Unsupervised anomaly detection

Real-time inference pipeline

