# Module 12 Report Template

## Overview of the Analysis

In this section, describe the analysis you completed for the machine learning models used in this Challenge. This might include:

* Explain the purpose of the analysis.
* Explain what financial information the data was on, and what you needed to predict.
* Provide basic information about the variables you were trying to predict (e.g., `value_counts`).
* Describe the stages of the machine learning process you went through as part of this analysis.
* Briefly touch on any methods you used (e.g., `LogisticRegression`, or any resampling method).

## Answers :
- This analysis tool uses datasets of historical lending activity from lending services company to build a model that can identify the creditworthiness of borrowers.

- Once the data is ingest from the dataset which includes multiple financial information (loan size, income, debt to income to name a few) its objective is to create a model that predicts the classification of the individual loans as "healthy" or "high risk" based on a rigorous supervised ML model assessment.

- The "target" variable (y) we're aiming at predicting for our analysis is the loan_status which can be classified as 0 or 1. All other data information are within the "features" variable (or X).

- The stages used as part of the machine learning process analysis used are:

*Create the model
*Fit the model
*Use the model
*Credit risk poses a classification challenge that’s inherently imbalanced since healthy loans easily outnumber risky loans. A supervised machine learning classification model which categorize according to shared qualities and characteristics using a Logistic Regression technic was used.
*To test the model a resampling of the dataset operation was and completed and re-test using the initial model to test the result and efficiency.

## Results

Using bulleted lists, describe the balanced accuracy scores and the precision and recall scores of all machine learning models.

* Machine Learning Model 1:
  
  * Accuracy: 0.9520479254722232
  * Precision: 1.0 / 0.85
  * Recall scores: 0.99 / 0.91


* Machine Learning Model 2:
  * Accuracy: 0.9936781215845847
  * Precision: 1.0 / 0.84
  * Recall scores: 0.99 / 0.99

## Summary

- Both precision for the logistic regression model, original and fit with oversampled data, were great at detecting healthy loans (1.0) and less accurate at detecting high-risk one (0.85 vs 0.84).

-In terms of the recall, the model using resampled data returned higher result at detecting healthy loan and high-risk loan alike (0.91 vs 0.99).

- To summarize, the model using resampled data as showed an overall increase in accuracy at detecting high-risk loan.

- As a side note, the balanced accuracy score was higher for the resampled data (0.9937 vs 0.9520), which echoes the classification report.

- To summarize, our model using the resampled data performs slightly better after comparing the accuracy score and classification report.

- Because of the nature of Credit risk which is inherently imbalanced since healthy loans easily outnumber risky loans it is imperative that our final model predict accuratly the "high-risk loan" or 0.

- At this preliminary stage of this tool and after analysing the results it would be our recommandation to continue our exploration of different supervised machine learning classification techniques such as "Support Vector Machines", "Decision Tree Based Algorithms" or "K-Nearest Neighbors" to name a few in order to increase the prediction accuracy level to 0.97 or higher.
