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


## 1) Load and clean data
* view data logs schema
![image1](https://github.com/AbdelrahmanGad/Sparkify_Udacity_ND/blob/main/1.PNG)

* remove corrupted rows as there is some rows having userid as empty string
![image1](https://github.com/AbdelrahmanGad/Sparkify_Udacity_ND/blob/main/2.PNG)
![image1](https://github.com/AbdelrahmanGad/Sparkify_Udacity_ND/blob/main/3.PNG)

