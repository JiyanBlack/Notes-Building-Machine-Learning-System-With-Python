# Visualization
* First step is visualization. Through visualization we can get many intuitions from the data.

# Build Classifiers
* The ingredients that makes a classification model:
  1. The structure of the model
  2. The search procedure
  3. The loss function(cost function)

# Training Error/Testing Error
* Training error is not reliable. Testing error is always higher than training error, but more convincible.
* Split data into two parts: training part and testing part.
* Use cross-validation to leverage the model with all data.
  1. Seperate the data into five different folds.
  2. Select one fold to be the test data.
  3. Train the model with other four folds.
  4. Get the accuracy for the test fold.
  5. Do it 5 times. Get the average accuracy.

# Train a multi-class classifier
* Achieve by using a classifier array(only one is True)
* By combined binary decisions
