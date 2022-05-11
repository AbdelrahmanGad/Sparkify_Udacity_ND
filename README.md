# Sparkify_Udacity_ND

## Project Description:
This is the Udacity Data Scientist Nanodegree Capstone project. The goal is to alter realistic datasets with Spark to create appropriate churn prediction characteristics. For the hypothetical music streaming service Sparkify (similar to Spotify and Pandora). The whole dataset was only available by subscribing for an AWS subscription, thus this project was done utilizing Udacity's workspace. A smaller.json dataset was given.

## Libraries:
* pyspark.sql
* pyspark.sql.functions
* pyspark.sql.functions
* matplotlib.pyplot
* pyspark.ml.feature
* pyspark.ml.classification
* pyspark.ml
* pyspark.ml.tuning
* pyspark.ml.evaluation

## Source Files:
* [Data](https://github.com/AbdelrahmanGad/Sparkify_Udacity_ND/blob/main/mini_sparkify_event_data.rar) : file containing event data log

## Project File:
* [Notebook](https://github.com/AbdelrahmanGad/Sparkify_Udacity_ND/blob/main/Sparkify.ipynb) : Jubyter notebook including all data manipulation ad analysis for this project

## Blog Post:
* [Blog Post](https://github.com/AbdelrahmanGad/Sparkify_Udacity_ND/blob/main/Sparkify_post.pdf) : rsulted blog post from analysis

## Results:
We developed a model to recognize churning customers of the Sparkify music streaming service for this project. To acquire a feel for the data, I first did some data exploration. After then, We started to add features. We trained (Logistic regression, Random forest classifier, Gradient boost and Decision tree) models once We obtained a dataset. The Random forest classifier had the best results.

I believe we can reach even better accuracy/F1 if we can search over a larger hyperparameter field for new users.

Finally, when mitigation steps are implemented and the user base grows and evolves, it is vital that this model be retrained frequently.

