Project_02 - Classification (Customer Churn)

Project Description
Description: The telecom operator Interconnect would like to forecast churn of their users.
Business Problem Statement: The company wants to forecast which users are planning to leave.
Business Value: To ensure loyalty, those who are planning to leave, will be offered with promotional codes and special plan options.

Taks Performed
1. Load necessary packages and datasets

2. EDA
* Check and correct datatypes
* Check and eliminate duplicate values
* Fill missing values
* Format column names
* Feature engineering
* Merge datasets into a single dataset
* Visualize the data (histogram, boxplots) to find seasonal trends and insights

3. Preprocess
* Apply one hot encoding
* Balance the two classes using SMOTE  from imblearn
* Split the dataset into train and test sets
* Apply MinMaxScaler

4. Train Classification Model
* Train a LightGBM classifier, using GridSearchCV to tune the hyperparameters

5. Evaluate Model Performance
* Check model accuracy, F1 score, and AUC ROC score
* Plot a confusion matrix to visualize the model accuracy
* Plot a ROC curve to visualize the model AUC ROC score
* Plot the feature importance graph

Conclusions
The feature importance analysis reveals that 'duration', 'monthlycharges' and 'totalcharges' emerge as the most influential factors affecting churn rate.
Notably, there appears to be a significant increase in churn within the first 1-1.5 years of customer enrollment (this was explored more deeply in the first EDA part of the final project).
To mitigate this churn propensity during the early years, a strategic approach involves offering promotional rates to newly acquired customers during this critical period.
By incentivizing loyalty through preferential pricing during the introductory phase, customers are more likely to develop brand familiarity and loyalty, thereby fostering a decline in churn rates.
