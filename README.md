# Jobathon-June-2022-Analytics-Vidhya

Problem Statement
A D2C startup develops products using cutting edge technologies like Web 3.0. Over the past few months, the company has started multiple marketing campaigns offline and digital both. As a result, the users have started showing interest in the product on the website. These users with intent to buy product(s) are generally known as leads (Potential Customers). 
Now, the marketing & sales team wants to identify the leads who are more likely to buy the product so that the sales team can manage their bandwidth efficiently by targeting these potential leads and increase the sales in a shorter span of time.

Now, as a data scientist, your task at hand is to predict the propensity to buy a product based on the user's past activities and user level information.

Approach
Initially the data was explored using EDA. The dataset was imbalanced with a class ration 95:5. Also most of the variables were categorical in the data. 
Date columns were extracted as year, month, week. Year was not relevant so only week was considered.
Missing vales were treated with constant imputation.

To balance the dataset, oversampling of train data was attempted using SMOTE, but did not improve model performance.
Transformation was performed on numerical columns.
Numerical variables were using Standard Scalar so the data works well with logistic regression, random forest and Artificial Neural Network.

ML Model building:
Logistic Regression, Random Forest, gradient Boosting and Artificial Neural networkalgorithms were evaluated. The results were verified using cross validation.
Logistic Regression, Random Forest, boosting algorithms gave almost equal performance but ANN gave much better performance.
ANN – There were three hidden layers of size 16/32/5. Dropout layers were also added to avoid overfitting.

