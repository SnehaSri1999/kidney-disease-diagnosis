# Kidney Disease Detection using Machine Learning

## Overview

Chronic Kidney Disease (CKD) is a progressive medical condition that can remain undiagnosed in early stages. This project builds a supervised machine learning pipeline to predict CKD using clinical patient data. The goal is to evaluate how effectively traditional machine learning algorithms can classify CKD risk from structured medical indicators.

The workflow includes data preprocessing, exploratory data analysis, feature preparation, model training, and comparative evaluation.

---

## Dataset

**Source:** UCI Machine Learning Repository – Chronic Kidney Disease Dataset  

- **Records:** 400 patient samples  
- **Features:** 24 clinical and physiological attributes  
- **Target Variable:** `classification` (ckd / notckd)

### Key Indicators

- Hemoglobin  
- Serum Creatinine  
- Blood Urea  
- Packed Cell Volume  
- Specific Gravity  
- Infection indicators (Bacteria, Pus Cells)

The dataset contains both numerical and categorical variables with missing clinical values, requiring preprocessing before modeling.

---

## Data Processing

The following preprocessing steps were implemented:

- Missing value handling using statistical imputation  
- Encoding categorical clinical variables  
- Feature scaling for model compatibility  
- Data cleaning and validation  

These steps ensure consistent feature representation for machine learning algorithms.

---

## Exploratory Data Analysis

EDA was performed to understand patterns in clinical indicators and CKD diagnosis.

### Analysis Included

- Distribution analysis using histograms  
- Outlier detection using boxplots  
- Feature relationships via correlation heatmaps  
- Class distribution analysis  

Clinical markers such as **serum creatinine, hemoglobin levels, and blood urea** showed strong correlation with CKD classification.

---

## Machine Learning Models

Three supervised learning algorithms were trained and evaluated:

- Logistic Regression  
- Support Vector Machine (SVM)  
- K-Nearest Neighbors (KNN)

Models were trained on processed features and evaluated on a held-out test dataset.

---

## Model Performance

| Model | Accuracy |
|------|------|
| Logistic Regression | 93.67% |
| Support Vector Machine (SVM) | 98.86% |
| K-Nearest Neighbors (KNN - k=22) | 96.00% |

The models achieved high accuracy due to strong separability among key clinical indicators.

---

## Tech Stack

### Programming
- Python

### Libraries
- pandas  
- numpy  
- matplotlib  
- seaborn  
- scikit-learn
