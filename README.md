# 1030project

This project is on using machine learning models to predict white wine quality score. Environment: data1030.yml
- python=3.10.5
- matplotlib=3.5.2
- pandas=1.4.2
- scikit-learn=1.1.1
- numpy=1.22.4
- xgboost=1.5.1
- shap=0.40.0
- jupyter_client=7.3.1
- jupyter_core=4.10.0
- jupyterlab=3.4.2
- jupyter_server=1.17.0
- jupytext=1.13.8
- rise=5.7.1
- plotly=5.8.0
- ipywidgets=7.7.0

# Data

Wine Quality Dataset by professor Paulo Cortez, on UCI Machine Learning Repository. Link: https://archive.ics.uci.edu/ml/datasets/Wine+Quality. This data set contains 4898 instances and 11 columns of explanatory variables and one column of target variables. The input features are continuous variables which represent numerical values from the lab results. The output variable is a numerical score based on the median of at least 3 evaluations from wine experts, who scored the wine quality between 0 and 10.

# Models

Ridge, Support Vector Machine, Random Forest, K-nearest neighbors, and Xgboost. 

# Results

The baseline RMSE of this problem is 0.886, which is from the result of using the mean of the target variable as my model prediction. The corresponding baseline
accuracy is 0.449. Random forest is the most predictive model for this problem. The optimal parameter choice of random forest is max_depth=100, max_features=0.25, n_estimators=1000, and other parameters are as default. It reached a RMSE of 0.607 and accuracy of 66.6% after rounding its predictions to the nearest integers.
