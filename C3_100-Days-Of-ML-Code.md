# 原文来自：[Avik-Jain/100-Days-Of-ML-Code](https://github.com/Avik-Jain/100-Days-Of-ML-Code)

# K Nearest Neighbours
## An intuition to K-NN Classification Algorithm

## What is K-NN?
K-Nearest Neighbor algorithm is a simple yet most used classification algorithm.
It can also be used for regression.
K-NN is non-parametric(means that it does not make any assumptions on the underlying data distribution),
instance-based(means that our algorithm doesn't explicitly learn a model.instead,it chooses to memorize the training instances.)
and used in a supervised learing setting.

## How Does K-NN Algorithm work?
K-NN when used used for classification -- the output is a class membership
(predicts a class -- a discrete value).
There are three key elements of this approach:
a set of labeled objects,e.g.,a set of stored records, a distance between objects,
and the value of k, the number of nearest neighbors.

## Making Predections
To classify an unlabeled object, the distance of this object to the labeled objects is computed,
tis k-nearest neighbores are identified, and the class label of the majority 
of nearest neighbors is then used to determine the class label of the object,
For real-valued input variables,the most popular distance measure is Euclidean distance.

## The Distance 
Euclidean dis tance is calculated as the square root of the sum of the 
squared differences between a new point and an existing point across all input 
attributes.
other popular distance measures include:
- Hamming Distance
- Manhattan Distance
- Minkowski Distance

## Value of k
Finding the value of k is not easy.A small value of k means that noise will have 
a higher influence on the result and a large value make it computationally expensive.
It depend a lot on your individual cases,sometimes it is best to run through each
possible value for k and decide for yourself.

<p align="center">
<img src="https://github.com/Avik-Jain/100-Days-Of-ML-Code/blob/master/Info-graphs/Day%207.jpg">
</p>
