# Predicting Blood Donation
About 5 million Americans need blood transfusion every year, and blood transfusion helps supply what our body is missing due to an illness or injury.

## Goal
The dataset is from a blood donation drive in Taiwan, where mobile blood donation vehicles drive to universities and collect blood. The goal of the project was to forecast if a donor will donate blood the next time a vehicle comes to a campus.

## Dataset
The dataset has 5 attributes with no missing values. All the attributes are numeric (integer), including the class value. This is how the first 5 rows of the dataset look like:
![Image](https://github.com/heydibyendu/Predicting-Blood-Donation/blob/master/data_head.png)

## Model Training
I trained Logistic Regression, KNN, SVM, Naïve Bayes, and Random Forest together with 10-fold cross-validation. Then I compared these models with their mean accuracy values in different cross-validation folds, using box and whisker plots. The results show a tight distribution for Logistic Regression with better mean accuracy, suggesting low variance.

## Results
The Logistic Regression model achieved 79.33% accuracy in predicting success through parameter estimation in the training set. I used grid search with 10-fold cross-validation for tuning the parameters. In the held-out validation set, the model achieved an accuracy of 79.14%, which matches closely to the expectations estimated during the tuning.
