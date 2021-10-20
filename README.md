# Credit Risk Analysis

## Overview

Credit risk is an inherently unbalanced classification problem, as good loans easily outnumber risky loans.

The credit card credit dataset from LendingClub (a peer-to-peer lending services company) was used for this analysis.

In this project, different techniques were used to train and evaluate models with unbalanced classes, such as the imbalanced-learn and scikit-learn libraries to build and evaluate models with resampling.

## Results

The results are listed below:

### 1. Naive Random Oversampling

![img](https://github.com/CarmenU18/Credit_Risl_Analysis/blob/main/Resources/Oversampling.PNG)

- Balanced Accuracy Test: 65%
- Precision High Risk: 1%
- Recall: 69%
- F1: 2%

### 2. SMOTE Oversampling

![img](https://github.com/CarmenU18/Credit_Risl_Analysis/blob/main/Resources/SMOTE%20Oversampling.PNG)

- Balanced Accuracy Test: 66%
- Precision High Risk: 1%
- Recall: 63%
- F1: 2%

### 3. Undersampling

![img](https://github.com/CarmenU18/Credit_Risl_Analysis/blob/main/Resources/Undersampling.PNG)

- Balanced Accuracy Test: 54%
- Precision High Risk: 1%
- Recall: 69%
- F1: 1%

### 4. Combination (Over and Under) Sampling

![img](https://github.com/CarmenU18/Credit_Risl_Analysis/blob/main/Resources/Combination%20(Over%20and%20Under)%20Sampling.PNG)

- Balanced Accuracy Test: 64%
- Precision High Risk: 1%
- Recall: 57%
- F1: 2%

### 5. Ensemble Learners

![img](https://github.com/CarmenU18/Credit_Risl_Analysis/blob/main/Resources/Ensemble%20Learners.PNG)

- Balanced Accuracy Test: 79%
- Precision High Risk: 3%
- Recall: 71%
- F1: 6%

### 6. Easy Ensemble AdaBoost Classifier

![img](https://github.com/CarmenU18/Credit_Risl_Analysis/blob/main/Resources/Easy%20Ensemble%20AdaBoost%20Classifier.PNG)

- Balanced Accuracy Test: 93%
- Precision High Risk: 9%
- Recall: 92%
- F1: 16%

The best model for our analysis was Easy Ensemble AdaBoost, with an accuracy test of 93%, precision of 9%, recall of 92% and F1 of 16%.

One model I would not use would be Undersampling as it has the lowest accuracy test.

When analyzing the data we found 3 variables that are not significant for our models, in all the data set the value is the same because it does not influence our target variable and therefore can be dropped:

- pymnt_plan
- hardship_flag
- debt_settlement_flag

Another reason that justifies the decision is that within the list of characteristics classified in descending order according to the importance of the characteristic, we can find these variables in last place.
