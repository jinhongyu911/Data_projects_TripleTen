Project_03 - Regression (Mining)

Project Description
Prepare a prototype of a machine learning model for Zyfra. The company develops efficiency solutions for heavy industry. The model should predict the amount of gold recovered from gold ore. You have the data on extraction and purification.
The model will help to optimize the production and eliminate unprofitable parameters. Parameters that are next to each other in terms of time are often similar. Some parameters are not available because they were measured and/or calculated much later.
That's why, some of the features that are present in the training set may be absent from the test set. The test set also doesn't contain targets. The source dataset contains the training and test sets with all the features.
You have the raw data that was only downloaded from the warehouse. Before building the model, check the correctness of the data.
We need to predict two values: rougher concentrate recovery and final concentrate recovery.

Taks Performed
1. Load necessary packages and datasets

2. EDA
* Check and correct datatypes
* Check and eliminate duplicate values
* Fill missing values
* Format column names
* Feature engineering
* Visualize the data (histogram, boxplots) to find seasonal trends and insights

3.  Train Regression Models and Evaluate Model Performances
* Train a Linear Regression model
* Evaluate model with cross validation using custom scoring functions
* Train Random Forest, Decision Tree models using GridSearchCV to tune the hyperparameters, utilizing custom scoring functions
* Graph and compare the three regression models

Conclusions
Upon fitting three distinct models, using the SMAPE score as the metric, the Random Forest Regressor showed the most favorable performance.
