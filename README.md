# Project 10 ENG: Traffic on highway

- The aim of this project is to explain the traffic on one of the highways for one-hourly intervals based on the training sample and generate predictions for all observations from the test sample
- Due to university requirements, the metric that was used to measure the predictive power of the model was **MAPE** (final score - 29%)
- The training set contained 29701 observations and 8 columns. During the data analysis process, categorical variables were split, additional interactions and variable transformations were introduced, which ultimately led to an expansion of the set to 31 columns
- The process of building the optimal model was based on **backward selection** in which insignificant variables with the highest p-value (significance level = 0.05) were dropped
- Performance was checked on 4 different algorithms: **Support Vector Regressor, Lasso/Ridge Regression and Elastic Net**
- In order to balance the results, the **StackingRegressor** algorithm was used, were Elastic Net was the **meta** regressor
