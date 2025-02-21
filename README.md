# credit-risk-classification

## Overview of the Analysis

This analysis aims to assess credit risk using a supervised machine learning model. Specifically, a logistic regression model was used to classify loans as either

## Results

* logistic regression model:
    * Accuracy: 99% (The model correctly classified nearly all loans.)
    * Precision for healthy loans (0): 1.00 (Virtually no false positives.)
    * Recall for healthy loans (0): 0.99 (Almost all actual healthy loans were detected.)
    * Precision for high-risk loans (1): 0.86 (Some high-risk loans were detected.)
    * Recall for high-risk loans (1): 0.94 (The model correctly identified most high-risk loans.)
    * F1-score for high-risk loans: 0.90 (Balanced performance between precision and recall.)

## Summary and Recommendation

Strengths:

* The model achieves a very high accuracy (99%), indicating strong predictive performance.
* Healthy loans (0) are classified with near-perfect precision and recall.
* High-risk loans (1) are identified well, with a recall of 94%, meaning most high-risk loans are correctly detected.

Weaknesses:

* The precision for high-risk loans is lower (0.86), meaning some risky loans are misclassified as healthy.
* If a lender wants to minimize financial risk, false negatives (misclassifying high-risk loans as healthy) should be reduced.

Recommendation:
* If high accuracy is sufficient, the logistic regression model is a strong candidate for credit risk classification.
* If minimizing lender risk is a priority, further improvements could be made by:
    * Adjusting the decision threshold for classification.
    * Exploring alternative models such as Random Forest or Gradient Boosting.
    * Applying oversampling techniques like SMOTE to balance the dataset.

Because the typical nature of credit analysis is to mitigate lender risk, I do not recommend this model.