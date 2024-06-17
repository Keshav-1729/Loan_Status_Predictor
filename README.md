# Loan Status Predictor

This repository contains the implementation of a machine learning project aimed at predicting the loan status of applicants. The project involves data preprocessing, visualization, model training, cross-validation, and hyperparameter tuning.

## Table of Contents

- [Project Description](#project-description)
- [Business Use Case](#business-use-case)
- [Data Preprocessing](#data-preprocessing)
  - [Data Cleaning](#data-cleaning)
  - [Data Visualization](#data-visualization)
- [Model Training](#model-training)
  - [Cross-Validation](#cross-validation)
  - [Hyperparameter Tuning](#hyperparameter-tuning)

## Project Description

This project aims to develop a model that predicts the loan status of applicants based on various features in the dataset. By accurately predicting loan statuses, financial institutions can make better lending decisions and manage risks more effectively.

## Business Use Case

Loan status prediction is a crucial task for banks and financial institutions. An accurate loan status predictor can:
- Reduce the risk of loan defaults by identifying high-risk applicants.
- Streamline the loan approval process by quickly evaluating applicants' creditworthiness.
- Optimize the loan portfolio by balancing approved and rejected loans.
- Enhance customer satisfaction by providing timely and fair loan decisions.

## Data Preprocessing

### Data Cleaning

Data cleaning was performed to ensure the dataset was free from inconsistencies, missing values, and irrelevant information. This step is crucial for maintaining the quality and accuracy of the model.

### Data Visualization

Data visualization techniques were used to explore the dataset and find correlations between features. This step helps in understanding the relationships and patterns in the data, which is essential for effective feature selection and model building.

## Model Training

### Cross-Validation

To generalize the model across the entire dataset and avoid overfitting, KFold cross-validation was used instead of the traditional train-test split. This method splits the dataset into multiple folds and trains the model on each fold, providing a more robust evaluation of the model's performance. 

The following models were trained and evaluated using KFold cross-validation:
- **Logistic Regression**: A statistical model that uses a logistic function to model a binary dependent variable.
- **Random Forest**: An ensemble learning method that uses multiple decision trees to improve classification accuracy.
- **Support Vector Machines (SVM)**: A supervised learning model that finds the hyperplane that best separates different classes in the feature space.
- **Multinomial Naive Bayes (MultinomialNB)**: A probabilistic model based on Bayes' theorem, often used for text classification and discrete features.

### Hyperparameter Tuning

Cross-validation was also used to perform hyperparameter tuning for the models. The following hyperparameters were tuned based on the cross-validation scores:
- **SVM's Kernel**: Different kernel functions (linear, polynomial, radial basis function) were evaluated to find the best-performing one.
- **Random Forest's n_estimators**: The number of trees in the forest was varied to find the optimal number for the best performance.
