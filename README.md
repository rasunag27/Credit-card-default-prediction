# Credit-card-default-prediction

**What is meant by default on credit card?**

Credit card default occurs when the user had failed to make the payment of the credit care for 180 days or as decided by the credit card company. Based on this, the issuer might assume that the user will probably not going to pay. At this point, the issuer might close the card, write off what user owe as bad debt and sell user account to a collectors agency.

**Objective**

To predict whether or not the a consumer will default on thier credit card with Machine learning approach using past data of credit card consumers. The goal is to achieve two things:
* Bring more consistency in the loaning process and
* Investigate what the key drivers are behind a potential defaulter.

*Source: www.towardsdatascience.com*

**Data desctiption**

* The dataset contains around 30000 observations with 25 variables extracted from a bank in Taiwan. Each observation corresponds to a particular credit card client.
* Among the 25 variables, 4 demographic variables are present (gender, age, marriage status and education). Financial variables of 6-months worth of payment data from April 2005 - September 2005 (amount of given credit, monthly repayment statuses, monthly amount of bill statements, and monthly amount of previous payments) are present.

**Exploratory Data analysis**

* In exploratory data analysis, data cleaning and data visualization is carried out.
* Based on target variable, visual analysis with respect to demographic data is done.
* Data variables are manipulated with correct names and categories as per the data description.

**Methodology**
* The problem is a classification problem and hence classification machine learning algorithms are used.
* One hot encoding is done for Education and Marriage demographic variable.
* Logistic Regression without scaling, Logistic Regression with scaling, Decision Trees and RandomForest algorithms are considered for prediciton.
* RandomizedSearchCV is implemented for the prediction of best parameters and then used those parameters for prediction.

**Metrics**
* Accuracy is first calcualted. Since accuracy is not a good metric for unbalanced dataset, just consideration is done.
* F1 score, ROC-AUC is used for metric evaluation. It can be seen that RandomForest with best parameters from RandomizedSearchCV shows an AUC of 0.77 compared to Decision Tree with 0.75 and scaled Logistic Regression with 0.5.

**Future development**

* The problem is implemented with unbalanced dataset itself.
* Recommendation is such that the data showed be made balanced first by using upsampling, downsampling or SMOTE technique and then proceed for machine learning algorithms.
* The metrics can be further imporved by using K-fold cross validation and so.




