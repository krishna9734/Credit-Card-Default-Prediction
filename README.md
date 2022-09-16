# Credit-Card-Default-Prediction

This project is aimed at predicting the case of customers default payments in Taiwan. From the perspective of risk management, the result of predictive accuracy of the estimated probability of default will be more valuable than the binary result of classification - credible or not credible clients. We can use the K-S chart to evaluate which customers will default on their credit card payments. Where we need to explore and analyze the data to forecast the “default payment next month” column for the test set.

In the first step, as for importing the raw data, the “default of credit card clients.xls” dataset has been loaded and created a data frame out of it. And then check over the statistical properties, know the shape and size of the dataset and perform data wrangling over It which includes converting the categorical features into object datatype, and handling NaN/ Null/ Missing Values of the data with visualization of the missing values as a matrix plot.

In the second step, performed the exploratory data analysis which discovers the relationships between the dependent variable ‘Defaulter’ and other features (e.g., ‘Gender’, ‘Education’, ‘Marital Status’, ‘Age’), the distribution and scatters plots of the bill amount and payment amount for both defaulter and non-defaulters’ month-wise, and checking the correlation between variables followed by the data visualization and data interpretation which involves finding patterns and dependency of variables.

In the third step, preprocessed the data through encoding (One Hot Encoding) the categorical features, selecting the best features (ANOVA F-test), treating anomaly and outlier values (Isolation Forest), handling class imbalance (SMOTE), handling data distribution imbalance (Standard Scaler), and splitting the data into train and test sets. After which data modeling for classifications takes place where the data fits through Logistic Regression, Random Forest classifier, Decision Tree classifier, KNN, Gradient Boosting, and XG Boosting classifier algorithms with evaluation parameters.

And at the last, the Supervised ML Classification project concluded by revealing that the XG Boosting classification model gave the best results with the highest Test Accuracy and F1 scores. From the feature importance, it is noted that the features 'payment_status_sept_2', 'payment_status_sept_0', and 'credit_limit' are the three most important factors as per Random Forest and XG Boosting algorithms that determine ‘Defaulters’.
