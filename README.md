# math_scores
The Jupyter notebook contains code to predict the math test scores (between 0 and 20 inclusive) of students from two secondary schools in Portugal. The features used to predict the math scores include students' behavior (e.g. amount of time spent studying), students' personal and family information (e.g. age, family size), and students' past academic performance. I one-hot encode all categorical variables before feeding them into the machine learning models.

Three machine learning models were used: linear regression, Lasso regression, and random forest regressor. Lasso regression, which picked 9 features and omitted the remaining 45 features, had the best performance on the test dataset, achieving a RMSE of 1.87. Linear regression came a close second, with a RMSE of 1.92. Random forest regressor had the worst performance on the test dataset, achieving a RMSE of 2.13.

On a side note, a simple correlation analysis revealed that past academic performance was highly correlated with the target variable. Surprisingly, behavioral variables such as the amount of time spent studying were not highly correlated with the target variable.

The dataset, which contains 395 student-level observations, was obtained from the UCI Machine Learning Repository: https://archive.ics.uci.edu/ml/datasets/student+performance
