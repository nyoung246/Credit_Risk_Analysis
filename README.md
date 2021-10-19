# Credit Risk Analysis

## Overview Of The Analysis

The purpose of this analysis is to employ different techniques to train and evaluate models with unbalanced classes. Several machine learning models were built to predict credit risk using the credit dataset from LendingClub. I oversampled the data using the RandomeOverSample and SMOTE algorithms,and undersample the data using the ClusterCentroids algorithm. Then a combinational was conducted using the SMOTEENN algorithm. Lastly, two machine learning models that reduce bias, BalancedRandomForestClassifier and EasyEnsembleClassifier, to predict credit risk was used.


## Results

The balanced accuracy scores and the precision and recall scores of all six machine learning models are as followed:
 
### Naive Random Oversampling
 
 ![Naive Random Oversampling_balanced](https://github.com/nyoung246/Credit_Risk_Analysis/blob/main/Resources/Naive%20Random%20Oversampling_balanced.PNG)

 ![Naive Random Oversampling](https://github.com/nyoung246/Credit_Risk_Analysis/blob/main/Resources/Naive%20Random%20Oversampling.PNG)
 
* Balanced accuracy Score: 0.65
* Precision Score High Risk: 0.01
* Precision Score Low Risk: 1.00
* Recall Score High Risk: 0.63
* Recall Score Low Risk: 0.66
 
 
### SMOTE Oversampling
 
  ![SMOTE Oversampling_balanced](https://github.com/nyoung246/Credit_Risk_Analysis/blob/main/Resources/SMOTE%20Oversampling_balanced.PNG)

  ![SMOTE Oversampling](https://github.com/nyoung246/Credit_Risk_Analysis/blob/main/Resources/SMOTE%20Oversampling.PNG)
  
* Balanced accuracy Score: 0.63
* Precision Score High Risk: 0.01
* Precision Score Low Risk: 1.00
* Recall Score High Risk: 0.60
* Recall Score Low Risk: 0.43
 
 
### Undersampling
 
  ![Undersampling_balanced](https://github.com/nyoung246/Credit_Risk_Analysis/blob/main/Resources/Undersampling_balanced.PNG)

  ![Undersampling](https://github.com/nyoung246/Credit_Risk_Analysis/blob/main/Resources/Undersampling.PNG) 
  
* Balanced accuracy Score: 0.63
* Precision Score High Risk: 0.01
* Precision Score Low Risk: 1.00
* Recall Score High Risk: 0.60
* Recall Score Low Risk: 0.43 
 
 
### Combination (Over and Under) Sampling
 
  ![Combination (Over and Under) Sampling_balanced](https://github.com/nyoung246/Credit_Risk_Analysis/blob/main/Resources/Combination%20(Over%20and%20Under)%20Sampling_balanced.PNG) 
  
![Combination (Over and Under) Sampling](https://github.com/nyoung246/Credit_Risk_Analysis/blob/main/Resources/Combination%20(Over%20and%20Under)%20Sampling.PNG)


* Balanced accuracy Score: 0.52
* Precision Score High Risk: 0.01
* Precision Score Low Risk: 1.00
* Recall Score High Risk: 0.69
* Recall Score Low Risk: 0.58
 
 
### Balanced Random Forest Classifier
 
  ![Balanced Random Forest Classifier_balanced](https://github.com/nyoung246/Credit_Risk_Analysis/blob/main/Resources/Balanced%20Random%20Forest%20Classifier_balanced.PNG) 

  ![Balanced Random Forest Classifier](https://github.com/nyoung246/Credit_Risk_Analysis/blob/main/Resources/Balanced%20Random%20Forest%20Classifier.PNG)
  
* Balanced accuracy Score: 0.79 
* Precision Score High Risk: 0.04
* Precision Score Low Risk: 1.00
* Recall Score High Risk: 0.67
* Recall Score Low Risk: 0.91
 
 
### Easy Ensemble AdaBoost Classifier
 
  ![Easy Ensemble AdaBoost Classifier_balanced](https://github.com/nyoung246/Credit_Risk_Analysis/blob/main/Resources/Easy%20Ensemble%20AdaBoost%20Classifier_balanced.PNG)

  ![Easy Ensemble AdaBoost Classifier](https://github.com/nyoung246/Credit_Risk_Analysis/blob/main/Resources/Easy%20Ensemble%20AdaBoost%20Classifier.PNG)
  
* Balanced accuracy Score: 0.93
* Precision Score High Risk: 0.07
* Precision Score Low Risk: 1.00
* Recall Score High Risk: 0.91
* Recall Score Low Risk: 0.94
  
  
## Summary

As seen in the results above, Easy Esemble AdaBoost Classifier has the highest balanced accuracy score of 0.93 and Combination (Over and Under) Sampling has the lowest balanced accuracy score of 0.52. Based on the results, I would recommend to the use the Easy Esemble AdaBoost Classifier model as it shows the best results out of all six machine learning models. This is because the result of 0.93 is the closest balanced accuracy score to 1 out of all the six models; and results that are nearest to the result of 1 show us the most accurate outcome. However, as the desired result would be the balanced accuracy score of 1, we should conduct more test to achieve a closer number.
