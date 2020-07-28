---
layout: post
title: Churn Model
subtitle: Identify what factors are causing customers to churn (leave) a telco business.
bigimg: /img/Telco-Blog-e1586208629167.jpeg
---

A telco, also known as a telephone service provider (Metro PCS, Sprint, T-Mobile, AT&T), is a business that deals with providing telecommunication services. Over the past 20 years, these companies have gone through an immense process of evolution to not only providing phone services, but also functioning as internet service providers.

The main goal of a telco business is to retain all the customers that are currently using the service and doing everything possible to ensure that a customer does not churn (leave) from the business. Therefore, it would be very beneficial for this type of business to be able to predict which type of customers are most likely going to leave and identify which factors contribute to it.

Being able to predict which customers will leave helps the business to especially cater to them by offering special promos and make sure they get the best customer service to encourage them to stay. If we can also understand the factors that cause customers to churn, it would give more insight into the problems of the business and would make it easier to implement improvements.

## Outline

Starting with the original dataset, it obviously had to be cleaned so that we can apply a model to it. First, all the unnecessary columns that we don't need were removed and we labeled the remaining columns as featured. For all the featured columns, the null values had to be either replaced or removed and the categorical features were one-hot encoded into binary 0 and 1 features. The features that were highly correlated also had to be dropped due to the fact that with high correlation, some features may have too much power into the outcome of the model applied. After creating the model, we want it to output the highest accuracy, so the hyperparameters are tuned to do so. In this case, the default scikit-learn values were used for all the parameters except for one, the learning rate which was set to 0.6.

## Results

* Customer tenure seemed to impact churn rate quite a bit -- this was potentially the most important feature. The longer a customer has been with us, the less likely they are to churn.
* Additionally, these customer attributes were correlated with churn:
    * Having multiple lines
    * Paying with an elctric check
    * Having no phone service
    * Having Streaming TV.
    * Having paperless billing
    * Having fiber optic internet service
* And, these customer attributes were negatively correlated with churn (in other words, correlated with customer retention):
    * Having online security
    * Having no internet service (streaming movies)
    * Having a one-year or two-year contract

## Evaluation

We evaluated our model on unseen test data and got a ROC AUC score of 0.858. This leads us to believe that our model will generalize well to future data.