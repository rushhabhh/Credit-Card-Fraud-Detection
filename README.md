# Credit-Card-Fraud-Detection
This repository contains a complete machine learning project aimed at detecting fraudulent credit card transactions using a real-world dataset. The project covers data cleaning, exploratory analysis, class imbalance handling with SMOTE, training multiple ML models, performance comparison, and visualizations to provide insights into fraud detection.

## Overview

The primary objective of this project is to build a reliable fraud detection system that can accurately classify transactions as fraudulent or legitimate. Since fraudulent transactions account for only ~0.17% of the dataset, special care is taken to address the class imbalance challenge.

This analysis is valuable for financial institutions aiming to prevent unauthorized transactions, reduce monetary losses, and improve customer trust through automated fraud detection solutions.

## Project Link

Access the full analysis and model evaluation in the Jupyter notebook provided in this repository.

Medium Article: [How I Built a Fraud Detection System with XGBoost and SMOTE](https://medium.com/@rvora3/how-i-built-a-fraud-detection-system-with-xgboost-and-smote-13cf2f3f7b18)

## Project Features

The project includes the following components:

**1. Data Exploration and Preprocessing**
- Dataset Overview: Based on Kaggle's credit card fraud dataset, featuring 284,807 transactions with PCA-transformed features.
- Class Imbalance: Only 492 transactions are labeled as fraud (~0.17%).
- Feature Summary: Includes Time, Amount, Class, and V1-V28 features anonymized using PCA.

**2. Exploratory Data Analysis (EDA)**
- Class Imbalance Visualization: Countplot to highlight skewed class distribution.
- Feature Distribution: Histograms of V1-V28, boxplots of Amount vs. Class.
- Time Patterns: Line plots of fraud vs legit transactions over time.

**3. Imbalance Handling with SMOTE**
- Oversampling: Synthetic Minority Oversampling Technique applied to balance training data.
- Training/Test Split: Stratified split to maintain class ratio.
  
**4. Machine Learning Models**
- Logistic Regression: Baseline model with high recall but low precision.
- Random Forest: High precision and balanced F1-score.
- XGBoost: Strong performance with best recall among models.

**5. Model Evaluation and Comparison**
- Metrics Used: Precision, Recall, F1-Score, and ROC-AUC.
- Confusion Matrices: Heatmaps for model predictions.
- Model Comparison: Bar and line plots to visualize metric scores across models.

## Dataset
**Source**: [Kaggle - Credit Card Fraud Detection](https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud)
**Records**: 284,807 transactions
**Fraud Cases**: 492
**Features**: 31 columns including PCA-transformed V1-V28, Time, Amount, and Class

## How to Use

To explore the project:

1. Clone or download this repository to your local machine
2. Create a virtual environment and activate it
3. Install the required packages
4. Ensure the dataset is available in the data directory
5. Open and run the Jupyter notebook
