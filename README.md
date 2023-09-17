# Credit Card Customer Churn
The objective of this project was to compare different machine learning models and select the one that predicts customer churn best using R.

# Introduction

Customer churn is a measure of lost customers, and minimizing churn can maximize a company's profits. The analysis focused on the purchasing behavior of bank customers using a specific dataset. The goal was to convert raw customer data into meaningful information and employ predictive data mining techniques to gain insights into customer churn.

# Data Description

The dataset used in this project contains information about banks and their existing and attrited customers. The target variable for prediction is the "Attrition Flag." The dataset consists of 10,127 rows and 21 columns.

Link to Dataset - https://www.kaggle.com/code/varunbarath/credit-card-customers-bank-churners/notebook

# Data Cleaning

Missing and duplicate values were checked and handled. The last two columns, which contained garbage values, were dropped as they were not useful for the models. Columns were also converted to numeric data for ease of training and testing the models.

# Exploratory Data Analysis

Several exploratory data analysis techniques were applied to gain insights into customer churn. The analysis included visualizations of attrition by gender, age, education, income, card type, and other factors.

# Principal Component Analysis

Principal Component Analysis (PCA) was used to reduce the dimensionality of the dataset. PCA helps in creating new variables that maximize variance while minimizing information loss. The dataset was standardized and normalized before applying PCA. The percentage of variation explained by each principal component was analyzed.

# Dimension Reduction

Based on the scree plot and cumulative proportion, the first 10 principal components were selected, explaining 95.713% of the variance. The last 4 principal components were dropped, reducing the model's dimensions from 19 to 15.

# Models

Different machine learning models were implemented and evaluated for predicting customer churn:

    Random Forest: Accuracy of 91.26% for dataset I and 96.35% for dataset II
    Logistic Regression: Accuracy of 90.07% for dataset I and 76.05% for dataset II
    SVM: Accuracy of 87.21% for dataset I and 86.86% for dataset II
    Naive Bayes: Accuracy of 89.78% for dataset I and 89.33% for dataset II
    Decision Tree: Accuracy of 88.74% for dataset I and 94.07% for dataset II

# Model Evaluation and Interpretation

Confusion matrices were used to evaluate the performance of each model. The accuracy percentages were calculated for all models and datasets.

# Conclusion

Based on the evaluation, the Random Forest model performed the best in predicting credit card customer attrition for both datasets. Naive Bayes and SVM showed slightly better performance with PCA data. It was observed that a dataset with 20 dimensions did not require PCA for dimension reduction. Time management and coordination were identified as challenges 
