colab.research.google.com# SummerAnalytics_Assignments
Summer Analytics Course by IIT Guwahati 2025
# AI-planet-hackathon
Hey! I am Tanisha Lalwani 👋
This is my submission for the AI Planet Hackathon.


# 🧠 NHANES Age Group Prediction Challenge (Hackathon2)

This repository contains a complete solution for the **NHANES Age Group Prediction** hackathon. The goal is to build a classification model that predicts whether an individual is an **Adult (0)** or a **Senior (1)** using health and demographic data from the NHANES dataset.

---

## 🚀 Problem Statement

Given health survey data, build a machine learning model to classify individuals into two age groups:

- **Adult (0)**
- **Senior (1)**

**Challenges addressed**:
- Missing values  
- Categorical variables  
- Class imbalance  
- Feature alignment across train/test sets

**Evaluation Metric**: F1 Score

---

## ⚙️ Tech Stack

| Tool          | Purpose                           |
|---------------|-----------------------------------|
| **Python 3.x** | Core programming language         |
| **Pandas**     | Data manipulation                 |
| **NumPy**      | Numerical computations            |
| **Scikit-learn** | Model selection, CV, metrics     |
| **LightGBM**   | Fast gradient boosting model      |
| **Jupyter Notebook** | Interactive model development |

---

## 🏗️ Architecture Flow

### ML Pipeline Overview

```mermaid
graph TD
    A[Start] --> B(Load Train/Test Data)
    B --> C(Exploratory Data Analysis)
    C --> D(Data Cleaning)
    D --> E(Feature Engineering)
    E --> F(Align Train/Test Features)
    F --> G(Model Training - LightGBM)
    G --> H(Hyperparameter Tuning)
    H --> I(Predict on Test Set)
    I --> J(Generate submission.csv)
    J --> K[End]
## How to Run the Notebook

1.  **Download Files**: Ensure you have `Train_Data.csv`, `Test_Data.csv`, and `submission_notebook.ipynb`.
2.  **Open in Google Colab**: Go to [colab.research.google.com](https://colab.research.google.com/), click `File` -> `Upload notebook`, and select `submission_notebook.ipynb`.
3.  **Upload CSVs to Colab Session**: In Colab, click the folder icon (Files tab) on the left sidebar, then click "Upload to session storage" to upload `Train_Data.csv` and `Test_Data.csv`.
4.  **Run All Cells**: Go to `Runtime` -> `Run all` to execute the entire notebook.

This will train the model, evaluate it, and generate `submission.csv` in your Colab session.

## Submission Summary

This submission presents a machine learning model to predict whether an individual is a 'Senior' (65+) or 'Adult' (under 65) based on the National Health and Nutrition Examination Survey (NHANES) dataset. The process involved robust data preprocessing, including imputation of missing values and one-hot encoding of categorical features. An XGBoost Classifier was trained with hyperparameter tuning, demonstrating strong internal validation metrics (Accuracy, Precision, Recall, F1-Score, and ROC AUC all at 1.0000). The `submission_.csv` file contains the model's predictions for the test set, formatted as required for the hackathon.