# Bank Customer Classification

## The Situation
You've just been hired as a Data Scientist for the Bank of Mavenland, the national bank in a country where data analysis is the most popular pastime.

## The Assignment
The product team at the bank wants to increase the company's revenue by reducing the number of people who leave, or "churn".
To help, you've been asked to build a classification model that identifies the customers at the highest risk of churn.

## The Objectives
1. Read in and explore the data
2. Prepare the data for modeling
3. Build & evaluate a logistic regression model
4. Build & tune a random forest model

## The Data Set

#### Bank Customer Churn
Account information for 10,000 customers at a European bank, including details on their credit score, balance, products, and whether they have churned.

#### Recommended Analysis
1. What attributes are more common among churners than non-churners? Can churn be predicted using the variables in the data?
2. What do the overall demographics of the bank's customers look like?
3. Is there a difference between German, French, and Spanish customers in terms of account behavior?
4. What types of segments exist within the bank's customers?

#### Objective 1: Profile & explore the data
Your first objective is to import the data and explore relationships between the features and target variable.

* Import the "Bank_Churn.csv" file and set an appropriate data type for each column.
* Check for missing values and calculate the min, max, and mean for numeric columns.
* Build a scatterplot matrix to find relationships between all pairs of numeric columns.
* Build box plots for each numeric column broken out by the target variable, "Exited".
* Build bar charts that show the percentage of "Exited" by category for each categorical column.

#### Objective 2: Prepare the data for modeling
Your second objective is to prepare the data for modeling through feature selection, feature engineering, and data splitting.

* Drop columns that aren't suitable for modeling from the dataset.
* Create a new column, "balance_to_income", by dividing "Balance" by "EstimatedSalary".
* Create a new column, "income_v_products", by dividing "EstimatedSalary" by "NumOfProducts".
* Create dummy variables for categorical columns.
* Split the data into train and test sets, with 20% of the rows in the test set.

#### Objective 3: Build & evaluate a logistic regression model
Your third objective is to fit a logistic regression model and evaluate it by using a confusion matrix, ROC curve, and precision & recall.

* Fit a logistic regression model on your training data.
* Build a confusion matrix to evaluate your model.
* Calculate accuracy, precision, recall, and F1 for your test data.
* Plot an ROC curve and calculate the AUC statistic.
* Plot precision and recall against the model threshold (set the threshold to the value where recall is the highest, but precision is still above 50%).

#### Objective 4: Fit & tune a random forest model
Your final objective is to fit a random forest model, tune it using cross validation, and evaluate test accuracy, AUC score, and feature importance.

* Fit a random forest model with default hyperparameters.
* Use cross validation to tune your model's hyperparameters.
* Report the final test accuracy and AUC score.
* Build a bar chart that shows feature importance.

#### [Project Link]()