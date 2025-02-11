##  XAI-based Income Prediction Using Logistic Regression (Explainable AI)

This repository contains a Jupyter Notebook implementing Explainable AI (XAI) techniques to analyze income prediction using the UCI Adult Income Dataset. The project includes data preprocessing, model training, evaluation, and SHAP-based explainability analysis.

### Dataset

The dataset used in this project is the UCI Adult Income Dataset, available here. It contains demographic and economic attributes used to predict whether an individual's income exceeds $50K per year.

### Features and Workflow

1. Data Preprocessing
- Load the dataset and handle missing values
- Encode categorical features using Label Encoding
- Standardize numerical features
- Split the dataset into training and testing sets

2. Model Training and Evaluation
- Train a Logistic Regression model
- Evaluate performance using:
- Accuracy score
- Confusion matrix
- Classification report
- ROC curve and AUC score

3. Explainability with SHAP
- Use SHAP (SHapley Additive exPlanations) for model interpretability
- Generate summary and force plots to understand feature contributions

4. Bias Mitigation
- Identify and remove bias-prone features (e.g., relationship, marital-status)
- Train and evaluate a new model with a reduced feature set
- Installation and Usage
- To run the notebook locally, follow these steps:

### Install dependencies:
- pip install -r requirements.txt
- Launch Jupyter Notebook:
- jupyter notebook XAI_3.ipynb

### Dependencies
- This project requires the following Python libraries: pandas, numpy, matplotlib, seaborn, scikit-learn, shap

## Install missing dependencies using:
pip install pandas numpy matplotlib seaborn scikit-learn shap

Results
- The logistic regression model achieved an accuracy of ~82%.
- SHAP analysis provided insights into the most influential features.
- Removing bias-prone features led to a trade-off between fairness and model accuracy.
