# -churn

## Telco Customer Churn Analysis & Prediction

A comprehensive end-to-end Machine Learning project for analyzing and predicting customer churn using the **Telco Customer Churn** dataset.

---

### 📌 Project Overview

Customer churn occurs when customers stop doing business with a company. Predicting customer churn allows telecommunication providers to proactively retain customers with targeted incentives, improved service plans, or personalized retention strategies.

This repository covers:
- **Exploratory Data Analysis & Preprocessing**: Handling categorical variables, missing values, and scaling.
- **Feature Engineering & Selection**: Applying dimensionality reduction and feature selection techniques to optimize model performance.
- **Classification Modeling**: Training and comparing various machine learning algorithms (Logistic Regression, Decision Trees, etc.).
- **Ensemble Techniques**: Boosting and bagging approaches (Random Forests, Bagging Classifiers) for improved generalization.
- **Model Evaluation**: Assessing models using Accuracy, Precision, Recall, F1-Score, ROC-AUC curves, and Decision Tree visualization.

---

### 📂 Repository Structure

```text
├── Classification/
│   ├── WA_Fn-UseC_-Telco-Customer-Churn.csv   # Telco Customer Churn Dataset
│   ├── Classification_Code.ipynb             # Baseline classification algorithms
│   ├── Classification_Code_(Plotting_DTs).ipynb # Decision Tree training & visualization
│   └── TL_Classification_Code.ipynb          # Detailed classification pipeline & metrics
│
├── Feature Engineering/
│   ├── FE_Chi Square.ipynb                   # Chi-Square test for categorical feature selection
│   ├── FE_LDA.ipynb                          # Linear Discriminant Analysis (LDA)
│   ├── FE_PCA.ipynb                          # Principal Component Analysis (PCA)
│   ├── FE_kPCA_QDA.ipynb                     # Kernel PCA & Quadratic Discriminant Analysis
│   ├── FE_RFE.ipynb                          # Recursive Feature Elimination (RFE)
│   ├── FE_SFS (sklearn).ipynb                # Sequential Feature Selection (scikit-learn)
│   └── FE_SFS (mlxtend).ipynb                # Sequential Feature Selection (mlxtend)
│
├── Ensemble/
│   └── Classification_Code_ensemble_added.ipynb # Ensemble learning models (Random Forest, Bagging)
│
├── .gitignore
└── README.md
```

---

### 📊 Dataset Details

The dataset used is the IBM Telco Customer Churn dataset (`WA_Fn-UseC_-Telco-Customer-Churn.csv`).

Key attributes include:
- **Demographics**: `gender`, `SeniorCitizen`, `Partner`, `Dependents`
- **Account Information**: `tenure`, `Contract`, `PaperlessBilling`, `PaymentMethod`, `MonthlyCharges`, `TotalCharges`
- **Services Subscribed**: `PhoneService`, `MultipleLines`, `InternetService`, `OnlineSecurity`, `OnlineBackup`, `DeviceProtection`, `TechSupport`, `StreamingTV`, `StreamingMovies`
- **Target Variable**: `Churn` (Yes / No)

---

### ⚙️ Prerequisites & Setup

Ensure you have Python 3.8+ installed along with the following libraries:

```bash
pip install numpy pandas scikit-learn matplotlib seaborn mlxtend
```

To run the notebooks locally:
```bash
jupyter notebook
```
Navigate to any notebook in `Classification/`, `Feature Engineering/`, or `Ensemble/` to run the analysis.
