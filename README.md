# Lung Cancer Detection using SVM


# Overview

This project aims to predict the likelihood of a patient having lung cancer based on various health and lifestyle factors using a Support Vector Machine (SVM) classifier. Early detection of lung cancer is crucial for timely treatment, and this model helps identify high-risk individuals using easily obtainable features like age, smoking habits, and common symptoms.

The dataset includes multiple patient attributes that may indicate lung health, lifestyle, and symptoms. By training an SVM model on this data, the project classifies patients into ‘Lung Cancer’ or ‘No Lung Cancer’ categories.

# Dataset

| Feature               | Description                                                  |
| --------------------- | ------------------------------------------------------------ |
| GENDER                | Patient's gender (Male/Female)                               |
| AGE                   | Patient's age in years                                       |
| SMOKING               | Smoking habit (Yes/No)                                       |
| YELLOW\_FINGERS       | Yellowing of fingers, often due to smoking (Yes/No)          |
| ANXIETY               | Presence of anxiety (Yes/No)                                 |
| PEER\_PRESSURE        | Influence of peers on smoking habits (Yes/No)                |
| CHRONIC DISEASE       | Presence of chronic diseases like diabetes or COPD (Yes/No)  |
| FATIGUE               | Feeling of tiredness or lack of energy (Yes/No)              |
| ALLERGY               | History of allergies (Yes/No)                                |
| WHEEZING              | Wheezing symptoms (Yes/No)                                   |
| ALCOHOL CONSUMING     | Regular alcohol consumption (Yes/No)                         |
| COUGHING              | Persistent coughing (Yes/No)                                 |
| SHORTNESS OF BREATH   | Difficulty in breathing (Yes/No)                             |
| SWALLOWING DIFFICULTY | Difficulty swallowing (Yes/No)                               |
| CHEST PAIN            | Pain in the chest (Yes/No)                                   |
| LUNG\_CANCER          | Target variable – indicates presence of lung cancer (Yes/No) |

# Why SVM?

Support Vector Machine (SVM) is a powerful supervised machine learning algorithm used for classification tasks. It works by finding the optimal hyperplane that separates data points of different classes with maximum margin.

Handles both linear and non-linear data effectively.

Robust to high-dimensional feature spaces.

Performs well for binary classification problems, making it ideal for predicting lung cancer (Yes/No).

# Project Steps

1.Data Loading

  Import the dataset using Python libraries like pandas.

2.Data Preprocessing

  Handle missing values (if any).

  Encode categorical variables (Label Encoding or One-Hot Encoding).

  Normalize/scale numerical features like AGE for better SVM performance.

3.Exploratory Data Analysis (EDA)

  Understand feature distributions.

  Visualize correlations between features.

  Detect patterns and insights that could influence model performance.

4.Model Training

  Split data into training and testing sets.

  Train an SVM classifier with an appropriate kernel (linear, RBF, or polynomial).

  Fine-tune hyperparameters using GridSearchCV or RandomizedSearchCV.

5.Model Evaluation

  Evaluate the model using metrics like:

  Accuracy,Precision,Recall,F1-Score, Confusion Matrix

  Check for overfitting or underfitting.

6.Prediction

  Use the trained model to predict lung cancer risk for new patients based on input features.


# Results

Accuracy: ~90–95% depending on dataset quality, feature preprocessing, and SVM kernel choice.

Recall (Sensitivity): High recall for positive cases is crucial to ensure lung cancer patients are correctly identified, minimizing false negatives.

Precision: Indicates reliability of positive predictions; higher precision reduces false positives.

Confusion Matrix: Typically shows the distribution of true positives, true negatives, false positives, and false negatives, highlighting model performance.

ROC-AUC: Values close to 1 indicate strong discriminative ability of the model in distinguishing between patients with and without lung cancer.

Interpretation: The SVM model effectively predicts lung cancer risk, with high sensitivity to detect positive cases, making it a valuable tool for early detection and clinical support.
