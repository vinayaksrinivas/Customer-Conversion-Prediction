# Customer-Conversion-Prediction
Problem Statement:
You are working for a new-age insurance company and employ mutiple outreach plans to sell term insurance to your customers. Telephonic marketing campaigns still remain one of the most effective way to reach out to people however they incur a lot of cost. Hence, it is important to identify the customers that are most likely to convert beforehand so that they can be specifically targeted via call. We are given the historical marketing data of the insurance company and are required to build a ML model that will predict if a client will subscribe to the insurance.

Features:
age (numeric)
job : type of job
marital : marital status
educational_qual : education status
call_type : contact communication type
day: last contact day of the month (numeric)
mon: last contact month of year
dur: last contact duration, in seconds (numeric)
num_calls: number of contacts performed during this campaign and for this client
prev_outcome: outcome of the previous marketing campaign (categorical: "unknown","other","failure","success")
Output variable (desired target):
y - has the client subscribed to the insurance?

Methodology:
Started with Data Cleaning, Encoded the target variable, performed EDA on every feature's distribution and its relationship with the target variable. Then, Splitted the data into testing and training data. Have performed scaling only on the training data. Then moving on to preprocessing the data to find out if the data is balanced or not. the result came up as imbalanced, thereby performed balancing of data. Later built 5 models -> Logistic Regression, KNN Algorithm, Decision Tree, Random Forest, XG-Boost. Found the hyper-parameter using stratified k fold method. Found the XG Boost to have the highest F1 Score. Thereby, implemented feature importance to this model and found the heirarchy of features.
