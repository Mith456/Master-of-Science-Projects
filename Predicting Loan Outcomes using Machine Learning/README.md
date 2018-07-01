# ABOUT DATA
	
This data comes from the Prosper p2p lending platform. I came across the data during the Udacity Data Analyst Nanodegree. 
All credit goes to Prosper and Udacity. A link to the data is here: https://s3.amazonaws.com/udacity-hosted-downloads/ud651/prosperLoanData.csv. 

The data contains a wide variety of information concerning loans on the Prosper p2p lending platform. 
This dataset is financial dataset and this is related to the loan, borrowers, lenders, interest rates and a few more.
Prosper Marketplace Inc. is a San Francisco, California based company specializing in loans at low interest rates to the borrowers.
In this dataset, we are using the data from the Prosper to analyze it and trying to find the pattern in the Prosper data. 
This may be tedious because of the sheer size of the dataset and the complicated nature of all the financial datasets. 

## MOTIVATION & OBJECTIVE

The motivation is to utilize the techniques and concepts of the Data Science for System Informatics class with a focus on learning and building good Machine Learning algorithms for large-scale Prosper loan dataset to classify its multi class loan status variable.
The main objective is to build a classification model to successfully predict which loans will default by computing the key high-performance metrics for the classifiers and observing the learning curve behavior of training and testing sets. Further objective is to lay emphasis on data preprocessing stages and on feature engineering to extract important features that aids our analysis in making better predictions. Focus will be laid on exploratory data analysis in the beginning to understand the behavior of the variables and assess importance of predictors with response variable.
Team members were interested in this project when we discovered this Udacity dataset, as this data will test Big Data challenge of a Financial Industry as an application of our data analysis skills, and felt that this would enable us to contribute in an important area of data science.

## INTRODUCTION TO THE PROBLEM SETUP
As the objective suggests, the problem here is to identify the entries which gets defaulted out of the 100000 entries. We setup a master dataset by cleaning the initial unprocessed data. Initial analysis begins with identifying the significant or affecting variables for the loan status and this happens through intuition, visualization, and research about the credit and loan sector. This helped us decide the key variables which have impact on the decision making.
Once the significant variables are identified, then comes the feature engineering techniques like dummies, feature hashing, and transformations on categorical variables to obtain their numeric representation.
The prime problem here was the dimension and the big data. This problem had a setup of Principal Component Analysis to deal with the former and a SGD partial fit classifier for the latter. Principal component analysis (PCA) is a technique used to emphasize variation and bring out strong patterns in a dataset. The partial fit estimator implements regularized linear models with stochastic gradient descent (SGD) learning: the gradient of the loss is estimated each sample at a time and the model is updated along the way with a decreasing strength schedule (aka learning rate).
Finally, a few chosen Machine learning classifiers are partially fit through SGD Classifier and their performance is computed through relevant metrics such as AUC, F1 Score and Recall. Classifiers were subjected to regularization by introducing ‘L1’ and ‘L2’ penalties. Parameter tuning was handled manually as the model was implemented through SGD partial fit. A learning curve was plotted to visualize the trend in the metrics over several chunk iterations. Best Classifier is chosen considering the high metric value and the behavior of the learning curve to judge the complexity and good model fit.



