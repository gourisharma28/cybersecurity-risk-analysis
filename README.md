# Cybersecurity-risk-analysis

## Project Overview

This project focuses on detecting cybersecurity threats using machine learning techniques. The objective was to classify network activity as either normal or malicious and evaluate the effectiveness of different classification algorithms in identifying cyber attacks.

## Tools & Technologies

* Python
* Pandas
* NumPy
* Scikit-learn
* Matplotlib
* Seaborn
* Jupyter Notebook

## Project Workflow

1. Data Cleaning and Preprocessing
2. Exploratory Data Analysis (EDA)
3. Model Development

   * Model 1 (bi-classification) : Logistic Regression
   * Model 2 (multi-classification): Random Forest
4. Model Evaluation

## Model Results

### Logistic Regression (Bi-classification)

The Logistic Regression model achieved excellent performance in distinguishing between normal and attack traffic. High precision, recall, and F1-scores across both classes indicate that the model successfully minimized both false positives and false negatives.

The confusion matrix further confirmed strong predictive performance, with the majority of observations correctly classified and very few misclassifications.

### Random Forest (Mutli-classification)

The Random Forest model performed well for identifying normal traffic and common attack categories. However, performance declined significantly for rare attack types.

Analysis of the confusion matrix revealed that the minority class *Rootkit* was consistently misclassified as normal traffic. This highlights a key challenge within the dataset: severe class imbalance and insufficient training examples for rare attack categories.

## Key Findings

* Logistic Regression demonstrated strong overall classification performance.
* Class imbalance had a significant impact on model performance.
* Rare attack categories were difficult to detect due to limited training samples.
* Traditional performance metrics can appear strong even when minority classes are poorly represented.
* Additional techniques such as class balancing, oversampling (SMOTE), or anomaly detection may improve detection of rare attacks.

