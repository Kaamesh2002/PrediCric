# PrediCric

## Objective:
To predict the final score of a batting team in an IPL cricket match using various machine learning algorithms.

## Preprocessing Steps:
### Removing Unwanted Columns:
Irrelevant columns that do not contribute to the prediction task were removed from the dataset. This helps in reducing noise and focusing on features that matter.

### Keeping Only Consistent Teams:
The dataset was filtered to include only teams that have consistently participated in the IPL. This ensures the model is trained on reliable and uniform data.

### Removing the First 5 Overs Data:
The first 5 overs of each match were excluded from the dataset. This decision focuses the model on the more significant middle and death overs where the scoring patterns are more consistent and predictive.

### Converting the 'Date' Column:
The date column was transformed from a string format to a datetime object. This conversion allows for easier manipulation and filtering based on time-related attributes, such as extracting the year for training and testing splits.

## Model Building:

### Linear Regression:
A fundamental model that provides a baseline for predicting the final score. It assumes a linear relationship between the features and the target variable.
### Decision Tree Regression:
A model that handles both linear and non-linear relationships by making splits in the data based on feature values. It can capture complex interactions between features.
### Random Forest Regression:
An ensemble method that builds multiple decision trees and combines their outputs to improve prediction accuracy. It reduces overfitting compared to a single decision tree.

### Adaptive Boosting (AdaBoost):
A powerful ensemble technique that improves model performance by focusing on the errors made by previous models. It iteratively adjusts the weights of data points and models, making the final model more robust and accurate.
