# 🏦 Loan Approval Prediction Model

**Author:** Eng. Abdallah Dwikat | **Date:** 9th September 2025

## 📝 Project Overview

This project involved developing a high-performance **machine learning model** to predict personal loan approval decisions. The goal was to identify key factors influencing approval and create a reliable classifier using a real-world financial dataset.

## 💻 Technical Skills Demonstrated

*   **Programming & Libraries:** `Python`, `Pandas`, `NumPy`, `Scikit-learn`, `Matplotlib`, `Seaborn`
*   **Data Preprocessing:** Data cleaning, feature encoding, correlation analysis, handling **class imbalance**.
*   **Data Visualization:** Created insightful heatmaps and distribution plots to understand data relationships.
*   **Machine Learning:** Built and evaluated a **Random Forest Classifier**.
*   **Model Evaluation:** Comprehensive analysis using `Accuracy`, `Precision`, `Recall`, `F1-Score`, `ROC-AUC`, and `Confusion Matrix`.

## 🚀 Process & Methodology

### 1. **Data Acquisition & Inspection**
*   Loaded and inspected a dataset of **4,269 loan applications** with 13 features.
*   Performed initial checks for missing values and data types, confirming a clean dataset.

### 2. **Data Preprocessing & EDA**
*   Standardized column names and string values to ensure consistency.
*   **Encoded categorical variables** (e.g., `Education`, `Loan_Status`) into numerical values.
*   Conducted **Exploratory Data Analysis (EDA)**, including a detailed correlation analysis using a custom heatmap. A key finding was that `cibil_score` (credit score) was the strongest predictor of loan approval.

### 3. **Handling Class Imbalance**
*   Identified a significant imbalance between approved and rejected loan classes.
*   Applied **oversampling techniques** to create a balanced dataset, ensuring the model would be trained without bias.

### 4. **Model Building & Training**
*   Segregated features and the target variable, removing non-predictive columns like `loan_id`.
*   Split the data into training and testing sets.
*   Instantiated and trained a **RandomForestClassifier** on the processed data.

## 📊 Results & Performance

The final model achieved **exceptional performance** on the test set:

| Metric | Score |
| :--- | :--- |
| **Accuracy** | **98.68%** |
| **Precision** | 0.99 |
| **Recall** | 0.98 |
| **F1-Score** | 0.99 |
| **ROC-AUC Score** | **98.70%** |

*   The **high ROC-AUC score** confirms the model's excellent capability to distinguish between classes.
*   The **confusion matrix** showed a minimal number of misclassifications.

## 🔑 Key Insight

The analysis proved that an applicant's **CIBIL score (credit score)** is the most critical factor in loan approval, a finding that aligns with real-world financial principles.
