# Loan_Status_Predictor
  In this Project, i used a dataset and performed the pre-processing of the dataset along with its data visualization to find correlation between the features.
  I used Logistic Regression, RandomForest , SVM and MultinomialNB to train the model and this time, i have avoided train_test_split and used the KFold cross validation instead to generalize the model all over the dataset and finding the score for all the splits.
  By using the cross validation, we can also perform hyper parameter tuning for the model.Here, i have done tuning in case of SVM's kernel and RandomForest n_estimators by looking at the cross_val_scores.
