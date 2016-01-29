# Intro to Machine Learning

Self-driving cars (SDC) is a good example of how machine learning works: similar to humans learning to drive, SDCs will learn from repeated exposure to examples of driving. 

> Examples provide 'features' from which to learn.

Features or attributes are extracted and used as index or references to aid classification of new objects. 

### Supervised Classification Examples 

1.  Given photo album, recognize someone in the pictures. 
2.  bank data: detect fraud? 
3. 	given someones musical choices, recommend other music 
4.  cluster Udacity students based on learning type. 

Examples one and three are supervised classification.  

Example two more of non-supervised, four is clustering. 

### Decision Surface 

Given a data on a scatter plot, the `decision surface (DS)` is the boundary dividing the two (N) classes.  "On the right side are all the blue dots, on the left side are all the red dots."

Allows us to generalize new data points into one class or the other.

## Naive Bayes

GaussianNB implements the Gaussian Naive Bayes algorithm for classification. The likelihood of the features is assumed to be Gaussian. via [scikit-learn.org](http://scikit-learn.org/stable/modules/naive_bayes.html#gaussian-naive-bayes)

```python

from sklearn import datasets
iris = datasets.load_iris()
from sklearn.naive_bayes import GaussianNB
gnb = GaussianNB()
y_pred = gnb.fit(iris.data, iris.target).predict(iris.data)
print("Number of mislabeled points out of a total %d points : %d"
...       % (iris.data.shape[0],(iris.target != y_pred).sum()))
Number of mislabeled points out of a total 150 points : 6
```

Using `fit()` and then `predict()` on the data set `iris`.

```python
def NBAccuracy(features_train, labels_train, features_test, labels_test):
    """ compute the accuracy of your Naive Bayes classifier """
    ### import the sklearn module for GaussianNB
    from sklearn.naive_bayes import GaussianNB
    from sklearn.metrics import accuracy_score
    gnb = GaussianNB()
    ### create classifier
    clf = gnb.fit(features_train, labels_train)

    ### fit the classifier on the training features and labels
    #TODO

    ### use the trained classifier to predict labels for the test features
    pred = clf.predict(features_test)


    ### calculate and return the accuracy on the test data
    ### this is slightly different than the example, 
    ### where we just print the accuracy
    ### you might need to import an sklearn module
    accuracy = accuracy_score(pred, labels_test)
    return accuracy
```

## Training and Testing

Key to provide disparate data sets.  Is easy to over-fit to your test dataset with small sample data. 

### Bayes Rule

Naive Bayes is a good algo for working with text identification.  Common to treat *each unique word* as a *feature*.

For parsing emails, each word in a writers vocabulary is a new feature.

 






