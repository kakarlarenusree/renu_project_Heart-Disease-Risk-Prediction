# Heart Disease Risk Prediction using Machine Learning
# Project Overview

This project aims to predict the likelihood of heart disease using machine learning techniques. The study applies classification algorithms to the Cleveland Heart Disease dataset to evaluate model performance and identify important clinical predictors. The project compares Logistic Regression, Random Forest, and XGBoost models, with a particular focus on model explainability using SHAP.

# Dataset

The dataset used in this project is the Cleveland Heart Disease dataset, obtained from the UCI Machine Learning Repository. It contains 303 patient records with 13 clinical features plus the target variable, including age, sex, chest pain type (cp), resting blood pressure (trestbps), cholesterol level (chol), fasting blood sugar (fbs), resting ECG results (restecg), maximum heart rate achieved (thalach), exercise-induced angina (exang), ST depression (oldpeak), slope of the ST segment, number of major vessels (ca), and thalassemia status (thal).

# Technologies Used
Python

Jupyter Notebook

Pandas

NumPy

Matplotlib

Seaborn

Scikit-learn

XGBoost

SHAP (SHapely Additive exPlanations)

Imbalanced-learn (SMOTE)

# Project Structure
heartdisease_final_code_for_review.ipynb – Main notebook containing analysis and model implementation

DS_project_FPR_Renu_updated_latest_to_review.docx – Final project report

README.md – Project documentation
# Methodology
1.Data loading and inspection

2.Exploratory Data Analysis (EDA)

	a.Univariate analysis

	b.Bivariate analysis

	c.Categorical feature analysis
	
	d.Correlation analysis
	
	e.Outlier detection

3.Data preprocessing
	
	a.Feature scaling
	
	b.Train-test split

	c.SMOTE for class imbalance handling

	d. Feature Scaling

4.Model implementation
	
	a.Logistic Regression
	
	b.Random Forest
	
	c.XGBoost

5.Hyperparameter tuning using GridSearchCV (5-fold cross-validation, optimised for ROC-AUC)

6.Model evaluation using accuracy, precision, recall, F1-score, ROC-AUC, and confusion matrices
# Results

The models were evaluated and compared across a three-stage framework (no SMOTE, SMOTE before tuning, and SMOTE with tuning) to assess the impact of class balancing and hyperparameter optimisation. XGBoost achieved the most consistent overall performance across accuracy, precision, recall, and F1-score, while Random Forest achieved the highest ROC-AUC. Logistic Regression remained a competitive, highly interpretable baseline.

# Model Explainability (SHAP)

To improve interpretability of the machine learning models, SHAP (SHapley Additive exPlanations) was applied to all three tuned models — Logistic Regression, Random Forest, and XGBoost. SHAP was used to:

Identify the most influential features affecting predictions (e.g., thal, ca, chest pain type, oldpeak, and maximum heart rate)
Understand how each feature increases or decreases the predicted risk
Provide both global feature importance rankings and local, per-patient explanations

This improves transparency and makes the models more suitable for healthcare applications where interpretability is critical.

# How to Run the Project
Clone the repository

Install required libraries

Open the Jupyter notebook

Run all cells to reproduce results

# Requirements

Install dependencies using:

### pip install pandas numpy matplotlib seaborn scikit-learn xgboost shap imbalanced-learn
# Author

Renusree Kakarla

# License

This project is for academic purposes only.
