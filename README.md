# Credit Risk Analysis
## Overview 
For this project, we used Python to build and evaluate several machine learning models to predict credit risk. All work were made in Jupyter Notebook.
The following procedure steps:

* Oversample the data using the RandomOverSampler and SMOTE algorithms.
* Undersample the data using the ClusterCentroids algorithm.
* Use a combinatorial approach of over- and undersampling using the SMOTEENN algorithm.
* Compare two machine learning models that reduce bias, BalancedRandomForestClassifier and EasyEnsembleClassifier.

Evaluate the performance of these models and make a recommendation on whether they should be used to predict credit risk.

## Resources:
Data Source: LoanStats_2019Q1.csv
Software: Python 3.9.7, Jupyter Notebook 6.4.5

## Random Over Sampler model
![](https://user-images.githubusercontent.com/101672943/186323239-5ee50c4a-3574-4965-9be3-a1da0bac9738.png)

The balanced accuracy score is 65%.

The high_risk precision is about 1% with 72% sensitivity which makes a F1 of 2% only.
Due to the high number of the low_risk population, its precision is almost 100% with a sensitivity of 68%.

## SMOTE model
![](https://user-images.githubusercontent.com/101672943/186323506-7f8bf093-9eb6-4305-872a-a547ed380421.png)
Result almost similar to our first model, only sensivity slitlly different
The balanced accuracy score is 66%.

The high_risk precision is about 1% with 63% sensitivity which makes a F1 of 2% only.
Due to the high number of the low_risk population, its precision is almost 100% with a sensitivity of 68%.

## Combination (Over and Under) Sampling
![](https://user-images.githubusercontent.com/101672943/186323941-50346dd5-709a-4415-aa66-a3e9cd29fe50.png)

##Balanced Random Forest Classifier & Easy Ensemble AdaBoost Classifier
![](https://user-images.githubusercontent.com/101672943/186324430-a6ad8a32-3a4d-4eb4-b1d5-918669727be8.png)

Unfortunatelly, for this model I received an AttributeError and wasn't able to complete an Balanced Random Forest & Easy Ensemble AdaBoost Classifier models...


# Summary
All the models used to perform the credit risk analysis show weak precision in determining if a credit risk is high.
With a low precision, a lot of low risk credits are still falsely detected as high risk which would penalize the bank's credit strategy and infer on its revenue by missing those business opportunities. Furthermore, the analysis wasn't compeleted so I cannot recommenedd or not recommened the bank to use any of these models to predict credit risk.



