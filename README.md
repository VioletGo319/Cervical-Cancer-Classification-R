# README - Prediction of Cervical Cancer Risk using Machine Learning

## Project Overview
This project by the VioletGo group aims to develop a predictive model for cervical cancer likelihood using medical and sexual history variables.

## Objective
Predict cervical cancer risk based on a range of medical and sexual history variables such as age, sexual partners, and diagnostic test results.

## Background

Cervical cancer remains a significant global health issue.
In 2008, 275,000 deaths were attributed to cervical cancer, with 88% in developing countries.
Persistent infection with high-risk HPV is a primary cause.
Early detection is crucial, especially in resource-limited areas.
Dataset

Contains data from 858 patients.
36 features, including demographic, medical history, and lifestyle factors.
4 target variables indicating cervical intraepithelial neoplasia or cervical cancer presence.
Approach

## Data Preprocessing

Mean imputation for missing values in continuous variables.
Random sampling for categorical variable imputation.
Feature standardization.
Risk score calculation based on four test results.
Data split: 80% training and 20% testing.
Exploratory Modeling

## Used LASSO regression for feature selection.
Baseline models: Linear Regression, Random Forest, K-NN, SVM, GBM.
Observed class imbalance which was addressed in the subsequent steps.
Downsampling

## Addressed class imbalance using downsampling.
Sensitivity analysis to test downsampling robustness.
Final Modeling

## Evaluated downsampling's impact on feature selection.
Performance evaluation of the five models across various downsampling ratios.
Evaluation

## Metrics used: MSE, RMSE, MAE, CV_MSE, CV_RMSE, CV_MAE, and Accuracy.
GBM outperformed other models with the highest accuracy of 0.835 on a 1:4 case-control ratio dataset.
SVM also showed promising results with an accuracy of 0.804 on the 1:3 case-control ratio dataset.
Linear Regression was the least effective.
Random Forest and KNN models showed moderate performance.
Sensitivity analysis confirmed stable performance across various case-control ratios.
Conclusion
The Gradient Boosting Machine model showed the best performance in predicting cervical cancer risk across different datasets. Future works might involve further model hyperparameter tuning, exploring additional feature engineering techniques, or exploring advanced machine learning algorithms.

## Usage

Install required libraries and dependencies.
Download the dataset and place it in the specified directory.
Run the preprocessing script to clean and prepare the data.
Execute the model script to train and evaluate the predictive model.
Use the trained model to predict on new data.
References
[1] Statistics on Cervical Cancer, World Health Organization, 2008.
[2] Role of HPV in Cervical Cancer, National Institute of Health, 2012.
[3] Source of the dataset used in the project.
