# Credit Card Default Prediction
[Code](https://github.com/SoumyaO/Credit-card-default-prediction/blob/main/CC%202.ipynb) | [Data](https://github.com/SoumyaO/Credit-card-default-prediction/tree/main/data)

## Description
The goal of this project was to predict the likelihood of default for a bank's customers and identify the key drivers that determine this likelihood. This information was then to be used to decide who to give credit to and what credit limit to approve. Additionally, it provided valuable insights into the bank's current and potential customers, guiding their future business strategies.

The dataset consisted of information of 25,000 existing clients of which 24,000 were used to study the likelihood of default and the 1,000 were randomly chosen as the test dataset.

A minimum viable product (MVP) was first developed with minimal data pre-processing to establish a baseline. The likelihood of default was modelled using logistic regression. The ROC (receiver operating characteristic) curve was plotted and the area under the curve (AUC) was computed.

Exploratory data analysis (EDA) was perfomed to identify and handle outliers and missing values, and comprehend data relationships. Using a correlation matrix, correlated regressors were identified and merged or eliminated. Categorical variables were one-hot encoded and numerical variables scaled and standardised. New features were engineered. EDA also revealed that the dataset was un-balances, with a smaller proportion of defaulters in comparison to non-defaulters. Therefore class-balanced sampling was done when fitting a model.Hyperparameter tuning through grid search was employed to optimize model parameters. Given the data's imbalance, F1 score was adopted as the performance metric for assessing the Logistic Regression model. The optimal threshold for classification was determined using Youden's J Statistic, which maximizes the difference between true positive rate and false positive rate across all possible threshold values. The model with the best ROC-AUC was chosen.
