# Risky Business - Classification Homework Assignment

![Credit Risk](Images/credit-risk.jpg)

## Assignment

Mortgages, student and auto loans, and debt consolidation are just a few examples of credit and loans that people seek online. Peer-to-peer lending services such as Loans Canada and Mogo let investors loan people money without using a bank. However, because investors always want to mitigate risk, a client has asked that you help them predict credit risk with machine learning techniques.

In this assignment I have built and evaluated several machine learning models to predict credit risk using data you'd typically see from peer-to-peer lending services. Credit risk is an inherently imbalanced classification problem (the number of good loans is much larger than the number of at-risk loans), so you will need to employ different techniques for training and evaluating models with imbalanced classes. You will use the [imbalanced learn](https://imbalanced-learn.readthedocs.io) and Scikit-learn libraries to build and evaluate models using the two following techniques:

1. [Resampling](#Resampling)
2. [Ensemble Learning](#Ensemble-Learning)

- - -

### Files

[Resampling Starter Notebook](Starter_Code/credit_risk_resampling.ipynb)

[Ensemble Starter Notebook](Starter_Code/credit_risk_ensemble.ipynb)

[Lending Club Loans Data](Starter_Code/Resources/LoanStats_2019Q1.csv.zip)

### Data
Resample the LendingClub data
- - -

### Objective:
Build and evaluate logistic regression classifiers using the resampled data.

### Resampling Notebook

#### Objectives:

1. Oversample the data using the `Naive Random Oversampler` and `SMOTE` algorithms.

2. Undersample the data using the `Cluster Centroids` algorithm.

3. Over- and undersample using a combination `SMOTEENN` algorithm.

For each of the above:

1. Train a `logistic regression classifier` from `sklearn.linear_model` using the resampled data.

2. Calculate the `balanced accuracy score` from `sklearn.metrics`.

3. Calculate the `confusion matrix` from `sklearn.metrics`.

4. Print the `imbalanced classification report` from `imblearn.metrics`.


#### Conclusions

* Which model had the best balanced accuracy score?



* Which model had the best recall score?
>
* Which model had the best geometric mean score?

### Ensemble Learning

In this section, I have trained and complated two different ensemble classifiers to predict loan risk and evaluate each model. I used the `balanced random forest classifier` and the `easy ensemble AdaBoost classifier`.

Completed the following steps for each model:

1. Train the model using the quarterly data from LendingClub provided in the `Resource` folder.

2. Calculate the balanced accuracy score from `sklearn.metrics`.

3. Print the confusion matrix from `sklearn.metrics`.

4. Generate a classification report using the `imbalanced_classification_report` from imbalanced learn.

5. For the balanced random forest classifier only, print the feature importance sorted in descending order (most important feature to least important) along with the feature score.

#### Conclusions

The balanaced random forest classifier and easy ensemble AdaBoost classifier provided results that were very similar with AdaBoost scoring marginally better. 

* Which model had the best balanced accuracy score?

* Which model had the best recall score?

* Which model had the best geometric mean score?

* What are the top three features?

#### Top Features for Balanced Random Forest Classifier

![Balanced Random Forest Classifier](Images/balancedrandomforest_feature.jpg)

#### Top Features for Easy Ensemble Classifier

![Easy Ensemble Classifier](Images/easyensemble_feature.jpg)
- - -

### Hints and Considerations

Use the quarterly data from the LendingClub data provided in the `Resources` folder. Keep the file in the zipped format and use the starter code to read the file.

Refer to the [imbalanced-learn](https://imbalanced-learn.readthedocs.io/en/stable/) and [scikit-learn](https://scikit-learn.org/stable/) official documentation for help with training the models. Remember that these models all use the model->fit->predict API.

For the ensemble learners, use 100 estimators for both models.

- - -

### Submission

- - -

© 2020 Trilogy Education Services, a 2U, Inc. brand. All Rights Reserved.
