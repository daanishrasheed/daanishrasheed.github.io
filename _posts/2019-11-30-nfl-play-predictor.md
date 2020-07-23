---
layout: post
title: NFL Play Predictor
subtitle: Predicting whether a team will run or pass
bigimg: /img/football.png
tags: [NFL]
---

Throughout its rich history, the NFL has turned into one of the most engaging yet most complicated sport of the modern era. For a team to be successful, there are many factors that can contribute in a variety of ways. Judging from the baseline, I can comfortably assume that the game has developed to a point where teams are relying on the passing game far more heavily than the run as offensive coordinators ran a pass play approximately 60% of the time.

Before beginning to apply a model on the data, I had to clean it by removing some columns and a few rows which, by my judgement, were deemed as unnecessary. One notable change I made was each column that contained text and were to be put through the model, I changed to numerical data. For example, my target column, PlayType, I made into a binary column because there were only 2 values that were possible to be predicted (Run or Pass). Changing text data into numbers resolved many issues that were occurring when trying to run a model on the data.

To find a model that would predict the most accurate results with respect to the data provided, I trained two machine learning alogorithms, Random Forest Classifier and XGBoost Classifier, on my data provided to me from the scikit learn package. I decided to go with the XGBoost Classifier, since it proved to be more accurate, and managed to derice the chart below:

![Chart](/img/weight-chart.JPG){: .center-block :}

