# Data Mining: Census Income Prediction Project

## Overview

This project explores the **Adult Dataset** (also known as the *Census Income* dataset) to predict whether an individual’s annual income exceeds **$50,000** based on demographic and employment-related attributes. This is a classic **binary classification** problem with real-world relevance to domains such as credit risk assessment, targeted marketing, and socio-economic analysis.

The goal of the project is not only to build predictive models, but also to demonstrate a complete **data mining pipeline**—from raw data cleaning to model evaluation.

---

## What I Accomplished

I designed and implemented an end-to-end machine learning workflow that processes raw census data and applies multiple algorithms to uncover patterns associated with higher income levels.

### 1. Data Cleaning & Preparation

- **Handling Missing Data:** Identified and removed records containing missing values (denoted as `"?"`) to ensure data quality.
- **Feature Engineering:** Converted categorical variables (e.g., education, occupation, marital status) into numerical form using **One-Hot Encoding**.
- **Data Binarization:** Transformed selected numerical features (such as age and hours worked per week) into binary categories based on their mean values to simplify pattern recognition for certain models.
- **Train/Test Separation:** Used predefined training and test splits provided by the dataset for fair evaluation.

---

## Machine Learning Models

To understand how different techniques perform on the same problem, I implemented and compared several models:

- **Baseline Models**
  - Decision Tree Classifier
  - Naive Bayes (BernoulliNB)

- **Similarity & Pattern-Based Models**
  - k-Nearest Neighbors (kNN)
  - K-Means Clustering (for exploratory pattern discovery)

- **Advanced Models**
  - Support Vector Machines (SVM)
  - Neural Networks (Multi-Layer Perceptron)

Each model was evaluated using accuracy metrics and confusion matrices to assess predictive performance and error patterns.

---

## Key Results

- **Best Overall Model:**  
  - **Support Vector Machine (SVM)** achieved the highest accuracy of **84.34%**.
- **Strong Alternative:**  
  - The **Neural Network** model achieved **81.89%** accuracy with consistent predictions.
- **Localized Accuracy:**  
  - For certain neighborhood sizes, **kNN** achieved accuracy levels of up to **90%** on specific test subsets.

These results demonstrate how model choice and feature representation significantly impact predictive performance.

---

## Tools & Technologies

- **Programming Language:** Python  
- **Libraries:**  
  - Pandas – data manipulation  
  - NumPy – numerical operations  
  - Scikit-learn – machine learning models and evaluation  
- **Environment:** Jupyter Notebook  
- **Data Source:** UCI Machine Learning Repository (Adult Dataset)

---

## How to Run the Project

1. Clone this repository.
2. Create and activate a virtual environment.
3. Install dependencies:
   ```bash
   pip install -r requirements.txt
