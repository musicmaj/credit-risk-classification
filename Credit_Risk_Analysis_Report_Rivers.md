# Module 12 Report 
Kade Rivers

## Overview of the Analysis

This Credit Risk Analysis Report was created to recommend the best model for predicting the outcome of a healthy loan or a high-risk loan based on a dataset which included current loans with a status of healthy or high-risk and the features of:  loan size, interest rate, borrower income, debt-to-income ratio, number of accounts, derogatory marks, and total debt. While the dataset itself is imbalanced due to the Healthy count being 75036 and the High Risk count being 2500, the machine learning process still allows for predictions and the accuracy and fit of those predictions is displayed with the various models referenced in the Jupyter Notebook provided.
Logistic Regression was the intended model for this report and assignment, however, other models including:  Decision Tree Classifier, Random Forest Classifier, Support Vector Classification, and KNeighbors Classifier were also trained and tested to determine which model had the best fit. The data was scaled prior to training and testing.

## Results

Listed below are the results of the above-named models.

Machine Learning Model 1: Logistic Regression
    * AUC: 0.996492776800469
    * Precision
        0 : 1.00
        1 : 0.87
    * Recall
        0 : 1.00
        1 : 0.98
    * f1-score
        0 : 1.00
        1 : 0.92
    * Accuracy: 0.99
    

Machine Learning Model 2: Decision Tree Classifier
    * AUC: 0.9382286902286903
    * Precision
        0 : 0.99
        1 : 0.87
    * Recall
        0 : 1.00
        1 : 0.81
    * f1-score
        0 : 0.99
        1 : 0.84
    * Accuracy: 0.99

Machine Learning Model 3: Random Forest Classifier
    * AUC: 0.9958956874033794
    * Precision
        0 : 1.00
        1 : 0.88 
    * Recall
        0 : 1.00 
        1 : 0.88
    * f1-score
        0 : 1.00 
        1 : 0.88 
    * Accuracy: 0.99

Machine Learning Model 4: Support Vector Classification
    * AUC: 0.9953770670078362
    * Precision
        0 : 1.00
        1 : 0.87 
    * Recall
        0 : 1.00
        1 : 1.00
    * f1-score
        0 : 1.00
        1 : 0.93
    * Accuracy: 1.00
    
Machine Learning Model 5: KNeighbors Classifier
    * AUC: 0.9960200010661548
    * Precision
        0 : 1.00
        1 : 0.87
    * Recall
        0 : 1.00 
        1 : 0.99
    * f1-score
        0 : 1.00 
        1 : 0.93
    * Accuracy: 1.00

## Summary

The top two models are the KNeighbors Classifier Model and the Logistic Regression Model. While the assignment was based on running the Logistic Regression Model, the KNeighbors Classifier was equally comparable and actually slightly more accurate in it's ability to predict the High Risk loans--which had far less representation in the data. It's arguable to use the KNeighbors Classifier to determine the Healthy vs High Risk loans in place of the Logistic Regression Model based on the Precision, Recall, f1-score, and Accuracy over the slight difference in the AUC. As more data is gathered, the models can be re-evaluated to determine if this is still the best course of action.
