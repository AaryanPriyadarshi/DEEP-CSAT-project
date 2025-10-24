#  DeepCSAT – E-Commerce Customer Satisfaction Prediction

## Project Overview
**DeepCSAT** is a data-driven machine learning project designed to predict **Customer Satisfaction (CSAT)** levels for e-commerce customer service interactions.  
By analyzing support records, agent performance metrics, and operational conditions, this project identifies the key drivers that impact customer experience.

---

## Domain
**Business / E-Commerce / Customer Analytics**

---

## Problem Statement
E-commerce companies often struggle to identify why customer satisfaction varies across service interactions.  
The objective of this project is to **predict customer satisfaction (CSAT scores)** using historical support data and to determine which factors — such as handling time, agent performance, or service conditions — have the greatest influence.  
This allows management to proactively improve agent training, response processes, and overall customer experience.

---

## Project Type
**Exploratory Data Analysis (EDA) / Classification / Explainable AI**

---

## Tech Stack
- **Programming Language:** Python  
- **Environment:** Google Colab  
- **Libraries Used:**
  - Data Handling → `pandas`, `numpy`
  - Visualization → `matplotlib`, `seaborn`, `plotly`
  - Machine Learning → `scikit-learn`, `xgboost`
  - Explainability → `shap`
  - Others → `scipy`, `logging`, `joblib`

---

## Workflow Summary

### **1. Import Libraries**
Imported all key libraries for data handling, visualization, machine learning, and explainability.

### **2. Dataset Loading**
- Loaded the dataset from Google Drive.
- Verified structure and previewed data.
- Confirmed presence of the **CSAT Score** target column.

### **3. Dataset Exploration**
- Checked dataset shape, data types, and missing values.
- Analyzed distributions and correlations among numerical features.
- Observed how agent ratings, response times, and conditions relate to satisfaction.

### **4. Input Validation**
- Verified that all necessary columns exist.
- Ensured structural integrity before preprocessing.

### **5. Data Visualization**
- Created exploratory plots to analyze feature relationships.
- Visualized agent and operational metrics using `seaborn` and `plotly`.

### **6. Feature Engineering & Preprocessing**
- Encoded categorical variables.
- Handled missing values using `SimpleImputer`.
- Scaled numerical data using `StandardScaler`.
- Split the dataset into training and testing subsets.

### **7. Model Training, Testing & Evaluation**
- Implemented two models: **Random Forest** and **XGBoost**.
- Normalized class labels for model compatibility.
- Evaluated performance using **accuracy**, **classification reports**, and **confusion matrices**.
- XGBoost achieved the best accuracy overall.

### **8. Feature Importance & Model Interpretation**
- Visualized the **Top 15 important features** influencing CSAT scores.
- Used **SHAP** to explain feature-level impacts on satisfaction predictions.
- Identified agent ratings, handling time, and tenure as the strongest predictors.

### **9. Model Saving**
- Saved the best model using `joblib` both locally and on Google Drive.
- Ensures model reusability and reproducibility.

### **10. Conclusion**
The **DeepCSAT** system successfully demonstrates how customer satisfaction can be modeled and explained through machine learning.  
By combining interpretability and predictive modeling, this project enables data-driven improvement in e-commerce customer service.
