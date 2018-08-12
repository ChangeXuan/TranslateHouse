# 原文来自：[Avik-Jain/100-Days-Of-ML-Code](https://github.com/Avik-Jain/100-Days-Of-ML-Code)

# 决策树
An intuition on decision tree for classification

## 什么是决策树?
It is a type of supervised learning algorithm that is mosyly used in classification
problems and works for both categorical and continuous input and output variables.

A decision tree is a tree in which each branch node represents a choice between a 
number of alternatives and each leaf node represents a decision.
- Here we've got an example with lots of points on our two dimensional scatter plot.
Now how does a decision tree work.
So what it is going to do us cut it up into slices in several iterations.
- We split the data and construct a decision tree side by side which we will use later.
This very task is achieved by using various algorthms.It builds a decision tree from a 
fixed set of examples and the resulting tree is used to classify future samples.
- The resulting Tree(obtained by applying algorithms like CART,ID3)which will be later used
to predict the outcomes.

## Decision tree algorithm:ID3
ID3 stands for iterative Dichotomizer 3. The basic idea is to construct the decision tree
by employing a top-down,greedy search through the given sets to test each attribute at every 
tree node.
Sounds simple - but which node should we select to build the correct and most 
precise decision tree? How would we decide that? Well,we have some measures taht can 
help us in selecting the best choice!


<p align="center">
  <img src="https://github.com/Avik-Jain/100-Days-Of-ML-Code/blob/master/Info-graphs/Day%2023.jpg">
</p>
