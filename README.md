# Ensemble-Techniques
### Definition: 
Ensemble methods combine several decision trees classifiers to produce better predictive performance than a single decision tree classifier. The main principle behind the ensemble model is that a group of weak learners come together to form a strong learner, thus increasing the accuracy of the model.

### Types of Ensemble Methods
1. Bagging
2. Boosting 
   * Ada Boost
   * Gradient Boost
   * Xg Boost

#### 1. BAGGing or Bootstrap AGGregating
Bagging is used when the goal is to reduce the variance(error on test data) of a decision tree classifier. Here the objective is to create several subsets of data from training sample chosen randomly with replacement. Each collection of subset data is used to train their decision trees. As a result, we get an ensemble of different models. Average of all the predictions from different trees are used which is more robust than a single decision tree classifier.
Advantages:
   * Reduces over-fitting of the model.
   * Handles higher dimensionality data very well.
   * Maintains accuracy for missing data.

Disadvantages:
   * Since final prediction is based on the mean predictions from subset trees, it won’t give precise values for the classification and regression model.




#### 2. Boosting
Boosting is used to create a collection of predictors. In this technique, learners are learned sequentially with early learners fitting simple models to the data and then analysing data for errors. Consecutive trees (random sample) are fit and at every step, the goal is to improve the accuracy from the prior tree. When an input is misclassified by a hypothesis, its weight is increased so that next hypothesis is more likely to classify it correctly. This process converts weak learners into better performing model.
Advantages:
   * Supports different loss function (we have used ‘binary:logistic’ for this example).
   * Works well with interactions.

Disadvantages:
   * Prone to over-fitting.
   * Requires careful tuning of different hyper-parameters.
   
   
### analysis 

Model           | Score
------------    | -------------
Random Forest   | 86.15%
Ada Boost       | 85.81%
Gradient Boost  | 86.48%
Xg Boost        | 86.46%

   
   
   
   
   

