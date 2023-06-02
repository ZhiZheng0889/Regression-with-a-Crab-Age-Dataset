## Day 2 Report: Regression-with-a-Crab-Age-Dataset

**Date:** [6/1/2023]  
**Project:** Regression-with-a-Crab-Age-Dataset

Today marked the second day of the Regression-with-a-Crab-Age-Dataset project. The primary focus of the day was on data preprocessing, feature engineering, and model selection using Optuna. Here is a summary of the tasks accomplished:

### Data Preprocessing:

1.  **Dataset Overview:** The day began by reviewing the Crab Age dataset, which consists of various features related to crabs and their ages. The dataset contained a mix of numerical and categorical features.
    
2.  **Handling Missing Values:** Missing values were identified and handled appropriately. In this dataset, missing values were found in the "Color" and "Weight" columns. The missing values in the "Color" column were imputed using the mode, while the missing values in the "Weight" column were imputed using the mean.
    
3.  **Encoding Categorical Variables:** Categorical variables, such as "Sex" and "Species," were encoded using one-hot encoding. This transformation ensures that categorical variables can be used as input for regression models.
    
4.  **Feature Scaling:** The numerical features in the dataset were standardized using the StandardScaler from scikit-learn. This step is essential to bring all features to a similar scale, preventing one feature from dominating the others during model training.
    

### Feature Engineering using Best Subset:

1.  **Best Subset Selection:** To identify the most informative features, a best subset selection approach was implemented. This method involves evaluating different combinations of features and selecting the subset that yields the best performance according to a chosen metric (e.g., R-squared or mean squared error).
    
2.  **Feature Combination Evaluation:** Various combinations of features were evaluated using a chosen regression model. For each combination, the model's performance was assessed through cross-validation or using a validation set.
    
3.  **Performance Comparison:** The performance of different feature combinations was compared based on the chosen evaluation metric. The subsets that yielded the highest performance were selected for further analysis.
    
4.  **Final Feature Subset:** After evaluating and comparing different feature combinations, the best subset of features was identified. This subset contains the features that have the most significant impact on predicting the crab age.
    

### Model Selection with Optuna:

1.  **Optuna Integration:** Optuna, a hyperparameter optimization framework, was used for model selection. Optuna automates the search for optimal hyperparameters by defining an objective function to minimize or maximize.
    
2.  **Model Evaluation:** Several regression models were considered for evaluation: XGBoost (XGBRegressor), LightGBM (LGBMRegressor), CatBoost (CatBoostRegressor), RandomForestRegressor, GradientBoostingRegressor, and LinearRegression. Optuna was used to search for the best hyperparameters for each model, optimizing the mean squared error (MSE) during the search process.
    
3.  **Cross-Validation:** To obtain robust estimates of model performance, k-fold cross-validation was implemented. The dataset was divided into k subsets, and each model was trained and evaluated on different folds, ensuring that the models were tested on unseen data.
    
4.  **Model Selection:** Based on the results of model evaluation and cross-validation, the model with the best performance was selected. Here are the results for each model:
    
    -   **XGBRegressor:**
        
        -   Best MSE: -4.2804424719193195
        -   Best parameters: {'n_estimators': 101, 'max_depth': 4}
    -   **LGBMRegressor:**
        
        -   Best MSE: -4.260125435923686
        -   Best parameters: {'n_estimators': 492, 'max_depth': 3}
    -   **CatBoostRegressor:**
        
        -   Best MSE: -4.269019251052433
        -   Best parameters: {'iterations': 409, 'depth': 5}
    -   **RandomForestRegressor:**
        
        -   Best MSE: -4.3045397941054135
        -   Best parameters: {'n_estimators': 348, 'max_depth': 10}
    -   **GradientBoostingRegressor:**
        
        -   Best MSE: -4.283166600577102
        -   Best parameters: {'n_estimators': 214, 'max_depth': 4}
    -   **LinearRegression:**
        
        -   Best MSE: -4.621136492962685
        -   Best parameters: {}

Overall, the second day of the Regression-with-a-Crab-Age-Dataset project was productive. Data preprocessing was performed, including handling missing values, encoding categorical variables, and feature scaling. Best subset selection was applied to identify the most informative features for predicting crab age. Model selection was performed using Optuna, considering several regression models such as XGBoost, LightGBM, CatBoost, RandomForestRegressor, GradientBoostingRegressor, and LinearRegression. The next steps will involve fine-tuning the selected model with the best performance and evaluating its performance on the test set.

_End of Day 2 Report._
