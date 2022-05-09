# Sparkify Churn Prediction
![image1](https://github.com/AbdelrahmanGad/Sparkify_Udacity_ND/blob/main/lc6raMp.jpg)

## Introduction 
Many firms fear churn. Some customers will naturally stop using the service, but too many can harm businesses regardless of revenue streams (ad sales, subscriptions, or a mix of both). With this in mind, organizations must be able to predict churn by identifying at-risk customers to avert customer loss.

Machine learning models trained on historical data can detect churn signals and predict them.


In this project, The challenge is forecasting which Sparkify music streaming customers will leave. I'll utilize Spark to build a machine learning model.


## Problem statment
Churn is a serious worry for many businesses. Some users will naturally cease utilizing the service, but if this number is too large, it can hurt businesses regardless of revenue sources (ad sales, subscriptions or a mix of both). With this in mind, the ability for businesses to predict churn by identifying at-risk clients is critical since it allows them to take steps to prevent the loss of customers, such as targeted offers or discounts.

Machine learning models built on historical data can help us understand churn signals and anticipate it before it happens.

Here the issue is predicting which Sparkify music streaming consumers would abandon the service. To accomplish this, I'll use Spark to create a machine learning model. Because there are only two possible outcomes, 'churn' and 'not churn,' we can use supervised learning to solve this binary classification problem.

## Metrics
The classification distribution is uneven since only 23% of users have the result churn. I picked the F1 Score measure, which is the harmonic mean of precision and recall, to account for this.


### 1) Load and clean data
* view data logs schema
![image1](https://github.com/AbdelrahmanGad/Sparkify_Udacity_ND/blob/main/1.PNG)

* remove corrupted rows as there is some rows having userid as empty string
![image1](https://github.com/AbdelrahmanGad/Sparkify_Udacity_ND/blob/main/2.PNG)
![image1](https://github.com/AbdelrahmanGad/Sparkify_Udacity_ND/blob/main/3.PNG)


### 2) Define churn
![image1](https://github.com/AbdelrahmanGad/Sparkify_Udacity_ND/blob/main/4.PNG)
![image1](https://github.com/AbdelrahmanGad/Sparkify_Udacity_ND/blob/main/5.PNG)

There is only 23% of users having churn flag


### 3) Exploratory Data Analysis
finding features that may affect churn flag

* Number of songs played
![image1](https://github.com/AbdelrahmanGad/Sparkify_Udacity_ND/blob/main/6.PNG)

* average on page events and selecting some features
![image1](https://github.com/AbdelrahmanGad/Sparkify_Udacity_ND/blob/main/7.PNG)

* average time user spend from registraion date
![image1](https://github.com/AbdelrahmanGad/Sparkify_Udacity_ND/blob/main/8.PNG)

* Length playsd songs
![image1](https://github.com/AbdelrahmanGad/Sparkify_Udacity_ND/blob/main/9.PNG)

### 4) Modeling
creating dataframe with label and features of interest
![image1](https://github.com/AbdelrahmanGad/Sparkify_Udacity_ND/blob/main/10.PNG)


### 5) Training multiple models and selecting best model
![image1](https://github.com/AbdelrahmanGad/Sparkify_Udacity_ND/blob/main/11.PNG)
based on performance for the modelswe selected random forest model
![image1](https://github.com/AbdelrahmanGad/Sparkify_Udacity_ND/blob/main/12.PNG)



## Conclusion
We developed a model to recognize churning customers of the Sparkify music streaming service for this project. To acquire a feel for the data, I first did some data exploration.
After then, We started to add features. We trained (Logistic regression, Random forest classifier, Gradient boost and Decision tree) models once We obtained a dataset. The Random forest classifier had the best results.

I believe we can reach even better accuracy/F1 if we can search over a larger hyperparameter field for new users.

Finally, when mitigation steps are implemented and the user base grows and evolves, it is vital that this model be retrained frequently.
