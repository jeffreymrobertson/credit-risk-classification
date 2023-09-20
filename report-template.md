# Module 12 Report Template

## Overview of the Analysis

In this section, describe the analysis you completed for the machine learning models used in this Challenge. This might include:

* Explain the purpose of the analysis.
* Explain what financial information the data was on, and what you needed to predict.
* Provide basic information about the variables you were trying to predict (e.g., `value_counts`).
* Describe the stages of the machine learning process you went through as part of this analysis.
* Briefly touch on any methods you used (e.g., `LogisticRegression`, or any resampling method).

## Results

Using bulleted lists, describe the balanced accuracy scores and the precision and recall scores of all machine learning models.

* Machine Learning Model 1:
  * The balanced score accuracy of the model is 94.4%
  * the precision score for the Healthy Loans is at 100% which makes sense considering there were a lot more healthy loans in the dataset.  However for High-Risk Loans the precision is only 87% meaning the model does not identify there are less True positives than expected
  * For recall the model predicts that a loan is high risk correctly 89% of the time 



* Machine Learning Model 2:
  * The balanced accuracy score for the second model is 99.6%.
  * The precision is still the same as the first model where it only identifies 87% of the high-risk loans
  * recall improves to 100% for high risk loans meaning there is less false positives then the first model

## Summary

Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. For example:
* Which one seems to perform best? How do you know it performs best?
The second model using the random oversampler seems to perform slightly better than the original as there are less false negatives which could affect the outcome on whether or not loan is deemed high risk.
* Does performance depend on the problem we are trying to solve? (For example, is it more important to predict the `1`'s, or predict the `0`'s? )
I believe it would be more important to identify the high-risk loans compared to the healthy loans.  for that reason the model needs to be capable of precisely identifying which is high risk.  In a business sense if a a decision is made to give a loan to someone who already has a high loan risk and the user bases the decision on the model it needs to be able to precisely identify 
If you do not recommend any of the models, please justify your reasoning.
i would not recommend either of the two models as I don't believe they are precise enough to identify high risk loans.  While the second model is better at identifying true positives from false positives, it is still not as precise as one would desire.