# House Prediction using Tree Ensemble Methods
## Introduction
This Kaggle project involved analyzing the Ames housing dataset to predict house prices based on various features. The goal was to conduct thorough Exploratory Data Analysis (EDA) and develop a robust machine learning model for accurate house price prediction. I managed to land in the <a href='https://www.kaggle.com/competitions/house-prices-advanced-regression-techniques/leaderboard'>top 25%</a> at the leaderboard on uploading my final submission file.

## File Descriptions
1) train.csv - The training set
2) test.csv - The test set
3) data_description.txt - Full description of each column, originally prepared by Dean De Cock but lightly edited to match the column names used here
4) sample_submission.csv - A benchmark submission from a linear regression on year and month of sale, lot square footage, and number of bedrooms
5) House Prices.ipynb - Notebook that generated submission used in Kaggle competition.
6) submission.csv - Final submission to Kaggle competition
7) Medium Article - Folder that contains files for my <a href="https://medium.com/@stevechesa/log-transforming-target-variables-and-enhancing-tree-ensembles-53be435d8041">Medium article</a> where I dive right in the effects of Log Transformation to Tree Ensemble Methods.

## Exploratory Data Analysis(EDA)
### Data Cleaning
  - Identified and handled missing values using imputation techniques appropriate for each feature 
  - Checked for availability of duplicated rows.

### Feature Engineering
  - Converted categorical variables into numerical representations using Ordinal Encoding.
  - Created new features from existing ones to capture more information (e.g., subtracting Year Built from Year Sold to get Age of house).

### Data Visualization
  - Used various plots (histograms, box plots and scatter plots) to understand the distribution and relationships of features with the target variable.
  - Identified key features that have the highest correlation with house prices.

## Model Development
### Model Selection
  - Evaluated different regression models including Random Forest Regressor, Extreme Gradient Boosting Regressor, CatBoost and LightGBM.

### Model Training
  - Split the dataset into training and test sets to evaluate model performance on unseen data.
  - Trained the selected models on the training set and applied hyperparameter tuning techniques.

### Model Evaluation
  - Evaluated model performance using metrics such as Mean Absolute Error (MAE), R^2 Score, and Root Mean Squared Error (RMSE).
  - Compared the performance of different models and stacked the best performing ones for final predictions.

## Outcome
The final model demonstrated high predictive accuracy on the test set where I got a score of 0.12935 on Kaggle and landed a top 25% position in the leaderboard. The project not only showcased advanced EDA and feature engineering techniques but also emphasized the importance of model selection and evaluation in building impressive predictive models.
