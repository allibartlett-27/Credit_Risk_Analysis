# Credit Risk Analysis

## Overview 
The purpose of this analysis was to take credit card credit data provided by LendingClub and use different resampling models to assess credit risk and determine whether our data should be used to predict credit risk. 

The resampling models we evaluated were oversample, undersample, as well as a combinatorial approach of over- and undersampling. These included RandomOverSampler, SMOTE, ClusterCentroids, and SMOTEEN algorithms. We also compared BalancedRandomForestClassifer and EasyEnsembleClassifer to reduce bias in our models and help us predict credit risk. 


## Results 

**Oversampling Algorithms**

* **Oversampling** - RandomOverSampler
  * Balanced Accuracy Score: 63.4%
  * Precision: 99%
  * Recall: 68%

* **Oversampling** - SMOTE
  * Balanced Accuracy Score: 64.7%
  * Precision: 99%
  * Recall: 63%

* **Undersampling** - ClusterCentroids 
  * Balanced Accuracy Score: 64.7%
  * Precision: 99%
  * Recall: 45%

* **CombinationSampling** - SMOTEENN
  * Balanced Accuracy Score: 52.9%
  * Precision: 99%
  * Recall: 57%

* **Ensemble Algorithm** - RandomForestClassifer
  * Balanced Accuracy Score: 78.8%
  * Precision: 99%
  * Recall: 91%

* **Ensemble Algorithm** - EasyEnsembleClassifer
  * Balanced Accuracy Score: 94.3%
  * Precision: 99%
  * Recall: 94%

## Summary 


