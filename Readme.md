 ![Alt text](knn.png?raw=true "KNN")

# Description of What the code does
This code shows how to use K-nearest neighbour classification model to train and predict on a dataset. 

The key lines are:

```
from sklearn.neighbors import KNeighborsClassifier
classifier = KNeighborsClassifier(n_neighbors = 5, metric = 'minkowski', p = 2)
classifier.fit(X_train, y_train)
```

Metric: Eucleadean distance
power : 2
No of neighbours to consider : 5

In the dataset, the x and y are age and estimated salary respectively. The purpose is to know whether a person buys the product or not and get an estimation.

# Few points on KNN:
 - In k-NN classification, the output is a class membership. An object is classified by a plurality vote of its neighbors, with the object being assigned to the class most common among its k nearest neighbors.
 - KNN is computation intensive. 
 - It is normally better than Logistic Regression, at least in this case.
 - Logistic regression is only a linear model so might result in lot of errors. But KNN is non-linear, so can capture more intricate areas in prediction.


