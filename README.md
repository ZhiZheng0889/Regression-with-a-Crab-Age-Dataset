# Regression-with-a-Crab-Age-Dataset
Playground Series - Season 3, Episode 16

#  Title: Age Prediction of Crabs using Machine Learning

## Abstract:

This project aims to predict the age of crabs based on various attributes such as sex, length, diameter, height, and different types of weights (total, shucked, viscera, shell). The data used for the competition is derived from a deep learning model trained on the original Crab Age Prediction dataset.

## Introduction:

The initial objective was to understand the problem statement and the data provided. The challenge required predicting the age of crabs, and the performance metric for the competition is yet to be decided.

## Data Exploration:

Upon initial data loading and inspection, we observed that the data set comprises of continuous and categorical features. The train set consists of 74,051 samples, while the original dataset has 3,893 samples.

Summary statistics for both the training set and the original dataset were computed. The features in the dataset include:

-   Sex: Gender of the crab - Male, Female and Indeterminate.
-   Length: Length of the crab (in feet).
-   Diameter: Diameter of the crab (in feet).
-   Height: Height of the crab (in feet).
-   Weight: Weight of the crab (in ounces).
-   Shucked Weight: Weight without the shell (in ounces).
-   Viscera Weight: Weight that wraps around the crab's abdominal organs (in ounces).
-   Shell Weight: Weight of the shell (in ounces).
-   Age: Age of the crab (in months).

Histograms were plotted for each feature to observe the distributions in both the training and original datasets. Additionally, correlation matrices were generated for the numeric variables.

## Data Preprocessing:

The data preprocessing step is yet to be carried out. It would involve handling missing values if any, encoding of categorical features, scaling of features, and possibly feature engineering.

## Model Building:

The next steps in the project would involve building a suitable machine learning model. Given the problem is a regression task (predicting the age of the crabs), algorithms like linear regression, decision tree regressor, random forest regressor, gradient boosting regressor, etc., could be tested.

## Future Work:

The following stages in the project would involve training the model, optimizing it using techniques such as hyperparameter tuning, and finally evaluating it. The objective is to build a model with the highest performance possible according to the competition metric.

The project's results will be updated once the model building, training, and evaluation stages are completed.

## Conclusion:

The data exploration stage has revealed interesting insights into the data, which will guide the subsequent steps in the project. The goal is to leverage these insights to build a robust machine learning model that can accurately predict the age of crabs.

----------

Please note that this report does not include any results from the model building, training, or evaluation stages as these steps are yet to be carried out. The report will be updated with these results once available.
