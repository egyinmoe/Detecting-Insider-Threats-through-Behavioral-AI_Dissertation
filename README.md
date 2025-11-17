🛡️ Detecting Insider Threats through Behavioral AI

A Machine Learning–Driven Approach for Identifying Insider Risk

This repository contains the code, dataset, and machine learning workflow used in a dissertation project on insider threat detection using behavioral data.

🔍 Project Overview

This repository contains the full implementation for the dissertation project “Detecting Insider Threats through Behavioral AI.”
The study investigates how machine learning (ML) and deep learning models can classify insider vs. non-insider behaviors using a simulated organizational log dataset.

The goal is to evaluate the performance of multiple algorithms, compare predictive capabilities, and reflect on the ethical considerations of deploying such technologies in real-world corporate environments.

🗂️ Repository Structure
📁 Detecting-Insider-Threats-through-Behavioral-AI_Dissertation/
│
├── Ver2_Insiderthreat_withgithub.ipynb   # Main modelling notebook
├── insider_logreg_baseline.pkl           # Saved Logistic Regression model
├── insider_random_forest.pkl             # Saved Random Forest model
├── README.md                             # Project documentation
│
└── (More files will be added gradually)

📊 Dataset Summary

The dataset used includes 12,000 behavioral activity records, representing both insider and non-insider users.

Key characteristics

Balanced target classes

6,000 insiders

6,000 non-insiders

Behavioral attributes

Activity type

Machine (PC) usage

File movement

Data size transferred

Personality scores

⚠️ Data Leakage Removal

The following fields were removed based on supervisor recommendation:

event_src — correlated with how logs were generated

date — temporal patterns gave unfair predictive advantage

Removing these ensures the models learn true behavioral patterns rather than hidden shortcuts.

🧠 Machine Learning Models Implemented

The modelling notebook implements and evaluates a suite of ML and DL algorithms:

Traditional ML Models

Logistic Regression

Random Forest Classifier

Support Vector Machine (RBF Kernel)

XGBoost Gradient Boosting

Deep Learning

Fully Connected Neural Network (Keras/TensorFlow

📈 Evaluation Metrics

Each model is evaluated using:

Accuracy

Precision

Recall

F1-Score

ROC-AUC

Confusion Matrix

This enables a reliable comparison of model strengths and weaknesses in detecting insider behaviors.

🛠️ How to Run the Notebook
Option A — Using Google Colab

Open the .ipynb file in Google Colab

Upload the dataset (AppliedResearchDataset_cleanVer1.csv)

Run all cells sequentially

View performance comparisons and saved model outputs

Option B — Local Jupyter Environment

Install required packages (scikit-learn, xgboost, tensorflow)

Open the notebook with Jupyter

Run the workflow end-to-end

🔍 Purpose of the Study

This research aims to:

Examine the feasibility of behavioral AI for insider threat detection

Compare multiple ML and DL methods in terms of predictive accuracy

Identify ethical risks (privacy, fairness, explainability)

Provide insights for responsible deployment in real organizations

📚 Citation

Ein Gyin Moe (2025). Detecting Insider Threats through Behavioral AI.
MSc Dissertation Project.

✨ Acknowledgements

This project was completed as part of the MSc in Information Systems with Computing (Business Analytics pathway).
Supervised by Terri, Dublin Business School.



