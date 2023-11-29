## Prediction of Cervical Cancer Risk using Machine Learning
#### Task: Classification
#### Topic: Machine Learning, Cervical Cancer Diagnosis
#### Language: R
### Project Overview
This project, developed by the VioletGo group, focuses on harnessing machine learning to create a predictive model for cervical cancer likelihood, grounded on variables related to medical and sexual history.

### Objective
To predict the risk of cervical cancer using variables such as age, sexual partners, and diagnostic test outcomes.

### Background
Cervical cancer stands as a prominent global health concern.
In 2008, it was responsible for 275,000 deaths, of which 88% occurred in developing countries1.
A primary cause is persistent infections linked to high-risk HPV2.
Emphasizing the critical nature of early detection, particularly in areas with limited resources.
### Dataset
Collated data from 858 patients.
Features: 36 in total, encompassing demographic details, medical history, and lifestyle choices.
Target Variables: 4 in total, signaling the presence of cervical intraepithelial neoplasia or cervical cancer.
### Approach
#### Data Preprocessing
Imputed mean values for absent data in continuous variables.
Adopted random sampling for imputation in categorical variables.
Undertook feature standardization.
Computed risk scores rooted in four test results.
Divided data into: 80% training and 20% for testing.
#### Exploratory Modeling
Employed LASSO regression to select pivotal features.
Established baseline models, including: Linear Regression, Random Forest, K-NN, SVM, and GBM.
Detected a skewed class distribution, prompting corrective measures in subsequent phases.
#### Downsampling
Rectified class imbalances via downsampling.
Conducted sensitivity analyses to verify the resilience of downsampling.
#### Final Modeling
Assessed the influence of downsampling on feature choices.
Gauged the efficacy of the five models over diverse downsampling ratios.
### Evaluation
Adopted Metrics: MSE, RMSE, MAE, CV_MSE, CV_RMSE, CV_MAE, and Accuracy.
Outstanding performance by GBM with an accuracy peak at 0.835, using a 1:4 case-control dataset.
SVM followed closely, registering an accuracy of 0.804 for a 1:3 case-control dataset.
Linear Regression lagged behind in efficacy.
Random Forest and KNN displayed average outcomes.
Sensitivity tests affirmed unwavering performance across different case-control datasets.
### Conclusion
The Gradient Boosting Machine (GBM) model emerged as the top performer in predicting cervical cancer risks, regardless of dataset variations. Potential future explorations could delve into fine-tuning model parameters, exploring innovative feature engineering methods, or testing advanced machine learning algorithms.

### Usage
Install the necessary libraries and dependencies.
Fetch the dataset and place it in the appropriate directory.
Execute the preprocessing script for data refinement and setup.
Run the model script for training and evaluation purposes.
Utilize the refined model for predictions on fresh data.
### References
World Health Organization's Statistics on Cervical Cancer, 2008 

Role of HPV in Cervical Cancer by National Institute of Health, 2012 
