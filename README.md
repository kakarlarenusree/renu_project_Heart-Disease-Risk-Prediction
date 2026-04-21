# Heart Disease Risk Prediction using Machine Learning
# Project Overview

This project aims to predict the likelihood of heart disease using machine learning techniques. The study applies classification algorithms to the Cleveland Heart Disease dataset to evaluate model performance and identify important clinical predictors. The project compares Logistic Regression, Random Forest, and XGBoost models.

# Dataset

The dataset used in this project is the Cleveland Heart Disease dataset obtained from the UCI Machine Learning Repository. The dataset contains 303 patient records with 14 clinically relevant features, including age, cholesterol level, chest pain type, and maximum heart rate.

# Technologies Used
Python

Jupyter Notebook

Pandas

NumPy

Matplotlib

Seaborn

Scikit-learn

XGBoost

# Project Structure
heartdisease_risk_prediction_project.ipynb – Main notebook containing analysis and model implementation

Heart_Disease_Report.docx – Final project report

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

4.Model implementation
	
	a.Logistic Regression
	
	b.Random Forest
	
	c.XGBoost

5.Hyperparameter tuning using GridSearchCV

6.Model evaluation using accuracy, precision, recall, F1-score, and confusion matrix
# Results

The models were evaluated and compared based on performance metrics. Ensemble methods such as Random Forest and XGBoost achieved higher accuracy compared to Logistic Regression, demonstrating improved predictive performance for heart disease classification.

# Model Explainability (SHAP)

To improve interpretability of the machine learning models, SHAP (SHapley Additive exPlanations) was used. SHAP helps explain individual predictions by showing the contribution of each feature to the model output.

In this project, SHAP was applied primarily to tree-based models such as Random Forest and XGBoost to:

Identify the most influential features affecting predictions (e.g., chest pain type, age, cholesterol level)
Understand how each feature increases or decreases the risk prediction
Provide global feature importance as well as local explanations for individual patient predictions

This improves transparency and makes the model more suitable for healthcare applications where interpretability is critical.

# How to Run the Project
Clone the repository

Install required libraries

Open the Jupyter notebook

Run all cells to reproduce results

# Requirements

Install dependencies using:

### pip install pandas numpy matplotlib seaborn scikit-learn xgboost
# Author

Renusree Kakarla

# License

This project is for academic purposes only.
