# PROBLEM OBJECTIVE
 
Training and testing datasets are provided for analysis. Training dataset has known class attributes, which we use to draw a best possible classifier model. This classifier model is used on the testing data without known class attribute to predict the classes with good consistency. 

## Data 

The given training data has 6136 instances, the class label is nominal attribute having three distinct labels. The data is imbalanced with different class types. Several techniques were applied in WEKA to balance the training dataset.

## Procedure
Upon applying the best filter to balance the training data, J-48 Decision tree and Random Forest Base Classifiers were tuned with different parameters by measuring key perfomance parameters like Accuracy and Balanced error rates between three classes. Meta-classifier such as Adaboost and Bagging were applied on Base Learners noting down the KPI's mentioned above to get the best model.
