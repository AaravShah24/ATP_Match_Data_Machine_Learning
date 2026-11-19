# ATP_Match_Data_Machine_Learning
This code uses 1171 matches of Jeff Sackmann's ATP Match data to train and evaluate models, as well as perform SHAP analysis. The goal of this project is to determine which features of match data most impact how a model predicts the outcome. First, the data is prepared for machine learning by removing all features that will not contribute to model prediction. After this ratios are calculated so that models do not inaccurately weight the sheer numbers in order to make predictions. Then, all the data is randomized and the features are renamed to prevent data leakage. After this, Random Forest Classifier, XGBoost, and Logistic Regression models are trained on this data. The Random Forest Classifier Model had an accuracy of 89.37%, the Logistic Regression Model had an accuracy of 90.06%, and the XGBoost model had an accuracy of 89.97%. Then, SHAP analysis was conducted on these models, and it yielded that for all three, 1st serve win percentage and 2nd serve win percentage were the factors that had the most impact on prediction. 

Data Source: Tennis Abstract / Jeff Sackmann ATP Match Data

License: The source dataset is distributed under the CC BY-NC-SA 4.0 license.

