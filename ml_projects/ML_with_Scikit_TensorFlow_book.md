# ML with Scikit and TensorFlow

##	Data Cleaning

<br>

## Data Exploration
-	Is there are any missing values...
-	Or values seem outdated. I need to check to see if it will affect the model later on -> see the predictors

## Select Data Model or Data for Modeling
Data set has many variables 
  - our brain is overfitting machine -> can't use intuition
  - PRIORITIZE USING STATISTIC to choose the best model ? (How -> scoring performance quality)
  - Best to split 1 big dataset into 3 (80/10/10) sets: trainning set, test set (never touch until the end of the project), validation set

Select The Predictor (Y)
  Predictor denotes as Y `y = df`
	Y is sually SERIES => using **dot-notation**
 
```
y = home_data.SalePrice 
#when home-data is DF and SalePrice is a column in that DF
```

Select Features (X, or labeled training data)
- The columns or attributes machine use train (
-	Sometimes, we use ALL COLUMNS, some cases we use fewer columns (this will depend on stakeholders and the outcome requirements)

```
Lay-man explanation:
I want to know how much seconds cats will come when they hear the pop-up sounds
Data I have: cat types, cat ages, times record, distance, container types
I want: times record - the results I want ML to give me - y
ML want: cat types,.. - all the data to work with - X

Sum up: ML trains X, used y to compare -> ML has X_train, y_train
But, in case ML "plagiarism", (I) take seperated data from the same set -> I have X_test, y_test
ML can do whatever, however many times in the process; I (X_test, y_test) won't involve until the end (final mark)
```

## Select Model: 
Used scikit-learn library (sklearn)
IMPORTANT: ask those following questions to build hypothesis and experiment.	
-	Define: What type of model will it be? A decision tree? Some other type of model? Some other parameters of the model type are specified too.
-	Fit: Capture patterns from provided data. This is the heart of modeling.
-	Predict: Just what it sounds like
-	Evaluate: Determine how accurate the model's predictions are.

In model: many ml models allow some `random_state` to ensure you get the same results in each run (model quality won't depend on value I chose). This is considered a good practice.
