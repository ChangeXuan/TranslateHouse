# 原文来自：[Avik-Jain/100-Days-Of-ML-Code](https://github.com/Avik-Jain/100-Days-Of-ML-Code)

# logistic regression

## what is logistic regression
logistic regression is used for a different class of problems known as classification problems.
Here the aim is to perdict the group to which the current object under observationbelongs to.
It gives you a discrete binary outcome between 0 and 1.
A simple example would be whether a person will vote or not in upcoming elections.

## How Does It Work?
Logistic Regression measures the relationship between the dependent variable 
(our label,what we want to predict) and the one or more independent variables
(our features),by estimation probabilities using it's underlying logistic function.

## Making Predictions
These probabilities must then be transformed into binary values in order to actually make a prediction.
This is the task of the logistic function,also called the sigmoid function.
This values between 0 and 1 will then be transformed into either 0 or 1 using a threshold classifier.

## Logistic vs Linear
Logistic regression gives you a discrete outcome but linear regression gives a continuous outcome.

## Sigmoid Function
the sigmoid-Function is an shaped curve thar can take any real-valued number and map it into a value between the range of 0 and 1,
but never exactly at those limits.

<p align="center">
  <img src="https://github.com/Avik-Jain/100-Days-Of-ML-Code/blob/master/Info-graphs/Day%204.jpg">
</p>
