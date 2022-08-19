# Module 12 Report Template

## Overview of the Analysis

In this section, describe the analysis you completed for the machine learning models used in this Challenge. This might include:

* Explain the purpose of the analysis.
* Explain what financial information the data was on, and what you needed to predict.
* Provide basic information about the variables you were trying to predict (e.g., `value_counts`).
* Describe the stages of the machine learning process you went through as part of this analysis.
* Briefly touch on any methods you used (e.g., `LogisticRegression`, or any resampling method).

The purpose of this analysis is to use techniques to train and evaluate models with imbalanced classes from credit risk data. Credit risk data is 
inherently imbalanced. The original data as well as a resampled dataset was created and evaluated against the original data. In both cases, a logistic
regression classifier was trained, the balanced accuracy score was calculated, and finally a confusion matrix and a classification report was generated.

Using both the original dataset and resampled data set, we wanted to predict the number of risky loans vs health loans. The original data contained 
75,036 healthy loands and 2,500 risky loans. The resampled data contained 18,765 health loans and 18,765 risky loans. Using both datasets, we
split the data into test and train data. The "y" was setup with the loan status data and the "X" was setup with all other data. A linear regression
model was instantiated and fit using the training data. From there the balance accuracy score was calculated, and a confusion matrix and well
as a classification report was generated.

## Results

Using bulleted lists, describe the balanced accuracy scores and the precision and recall scores of all machine learning models.

* Machine Learning Model 1:
  * Description of Model 1 Accuracy, Precision, and Recall scores.

* For model 1, the accuracy was scored at 94.3%, indicating a high level of accuracy. 
* The precision was calculated to be 97.1% (55,999 / (55,999 + 1,676), which represents a high confidence
that the model correctly made positive predictions. 
* The recall was calculated to be 99.5% (55,999 / (55,999 + 205), indicating a high condifence that the model correctly categorized the transactions.

* Machine Learning Model 2:
  * Description of Model 2 Accuracy, Precision, and Recall scores.
  
* For model 2, the accuracy was scored at 94.5%, indicating a high level of accuracy. 
* The precision was calculated to be 96.8% (55,964 / (55,964 + 1,872), which represents a high confidence
that the model correctly made positive predictions. 
* The recall was calculated to be 99.9% (55,964 / (55,964 + 9), indicating a high condifence that the model correctly categorized the transactions.

## Summary

Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. For example:
* Which one seems to perform best? How do you know it performs best?
* Does performance depend on the problem we are trying to solve? (For example, is it more important to predict the `1`'s, or predict the `0`'s? )

If you do not recommend any of the models, please justify your reasoning.

Both models seemed to perform at a high level of accuracy and confidence. Either model will be accurate for predicting healthy loans and 
risky loans. The performance of each model may depend on the problem that is being solved.