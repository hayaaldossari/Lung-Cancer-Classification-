# Lung-Cancer-Classification

## Overview
This project focuses on developing a **machine learning classification model** for diagnosing lung cancer.  
The goal is to predict whether a patient has lung cancer (and its severity level) based on clinical features.  

We implemented and compared multiple algorithms:
- **Support Vector Machine (SVM)**
- **Logistic Regression**
- **Random Forest Classifier**

Through evaluation and experimentation, our objective is to identify the most effective model for lung cancer detection, which can potentially assist healthcare professionals in making more accurate diagnoses.



## Dataset
- The dataset contains patient medical records and cancer levels.
- Target variable: **`level`** (Low, Medium, High).
- Preprocessing steps:
  - Removed unnecessary columns (`Patient Id`).
  - Converted categorical levels into numeric values:
    - Low → `0`
    - Medium → `1`
    - High → `2`
  - Cleaned column names (lowercase, replaced spaces with underscores).
    dataset link :https://www.kaggle.com/datasets/m5anas/cancer-patient-data-sets





## Project Workflow
1. **Data Preprocessing**
   - Cleaned column names.
   - Handled target encoding for cancer levels.
   - Split dataset into training (70%) and testing (30%).

2. **Data Visualization**
   - Pie chart for cancer level distribution.
   - Correlation heatmap to analyze relationships between features.

3. **Model Training & Evaluation**
   - Trained multiple ML models: SVM, Logistic Regression, Random Forest.
   - Evaluated models using:
     - Accuracy Score
     - Confusion Matrix
     - Classification Report
     - F1 Score
     - Log Loss

4. **Model Comparison**
   - Accuracies are stored and compared to find the best performing model.



## Results
- **SVM**: Linear kernel used for separating cancer levels.
- **Logistic Regression**: Baseline linear model.
- **Random Forest**: Provided robust classification with high accuracy.

Evaluation metrics (accuracy, confusion matrix, F1 score) showed that **Random Forest** achieved the best overall performance.



## Requirements
Install required libraries before running the code:

```bash
pip install numpy pandas matplotlib seaborn scikit-learn

```bash
pip install numpy pandas matplotlib seaborn scikit-learn
