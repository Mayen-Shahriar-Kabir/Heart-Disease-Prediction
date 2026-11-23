# 🫀 Heart Disease Prediction & Severity Classification

This repository contains a machine learning pipeline designed to predict the presence and severity of heart disease based on clinical and demographic features. Developed as part of the **CSE422** coursework, the project explores the end-to-end data science lifecycle, from exploratory data analysis and handling imbalanced datasets to model training and performance evaluation.

### 🔬 Project Overview
The objective of this classification task is to categorize patients into varying risk levels (0-4) to assist healthcare professionals with data-driven diagnostic support. The dataset consists of 920 patient records with 15 clinical features, including resting blood pressure, serum cholesterol, and exercise-induced angina.

**Key Challenges Addressed:**
* **Missing Data & Encoding:** Handled missing values via median/mode imputation and applied label encoding for categorical variables.
* **Class Imbalance:** Analyzed and managed a highly imbalanced target variable to prevent model bias.
* **Feature Engineering:** Utilized Pearson, Spearman, and Kendall correlation methods to identify the strongest predictors (e.g., fluoroscopy colored vessels and ST depression).

### 🛠️ Methodology & Tech Stack
* **Data Processing:** Python, Pandas, NumPy, Scikit-learn (StandardScaler, SimpleImputer, LabelEncoder)
* **Visualization:** Matplotlib, Seaborn (Correlation Heatmaps, Density Plots, Boxplots)
* **Supervised Learning Models:** 
  * K-Nearest Neighbors (KNN)
  * Logistic Regression
  * Neural Networks (MLPClassifier)
* **Unsupervised Learning:** K-Means Clustering (k=3) for exploratory grouping.

### 📊 Results & Model Selection
Three supervised models were tuned using Grid Search and 5-fold cross-validation. 
* The **Neural Network (MLPClassifier)** achieved the most balanced performance with an F1-Score of 57.90% and a Precision of 59.79%.
* The project highlights the precision-recall tradeoff inherent in medical diagnostic models and demonstrates rigorous evaluation using Confusion Matrices and ROC Curve Area Under Curve (AUC) scoring.

### 📄 Full Documentation
For a comprehensive breakdown of the exploratory data analysis, network analysis, and validation metrics, please refer to the attached `Project_Report.pdf`.
