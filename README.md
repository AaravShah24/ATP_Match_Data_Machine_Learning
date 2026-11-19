# ATP_Match_Data_Machine_Learning
This code uses 1,171 matches of Jeff Sackmann's ATP Match data to train and evaluate machine learning models, as well as to perform SHAP analysis to determine which match statistics have the most impact on how the models predict match outcomes. To prepare the data, features which have no impact on the match are removed, and then large raw numbers are converted into ratios so that the models evaluate relative performance rather than forming biases based on sheer volume. After this, data leakage is prevented by renaming columns in the data and randomizing player assignments before training the models. The three models used in this project are Random Forest Classifier, XGBoost, and Logistic Regression, which resulted in accuracies of 89.37%, 89.97%, and 90.06% respectively. SHAP analysis is then conducted on these models, and the results yield that 1st serve win percentage and 2nd serve win percentage had the most impact on the model's prediction of the outcome of the match. 

Data Source: Tennis Abstract / Jeff Sackmann ATP Match Data

License: The source dataset is distributed under the CC BY-NC-SA 4.0 license.

