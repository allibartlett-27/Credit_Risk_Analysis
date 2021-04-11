# Credit Risk Analysis

## Overview 
The purpose of this analysis was to take credit card application data provided by LendingClub and use different resampling models to assess credit risk and determine whether our data should be used to predict credit risk. 

The resampling models we evaluated were oversample, undersample, as well as a combinatorial approach of over- and undersampling. These included RandomOverSampler, SMOTE, ClusterCentroids, and SMOTEEN algorithms. We also compared BalancedRandomForestClassifer and EasyEnsembleClassifer to reduce bias in our models and help us predict credit risk. 


## Results 

**Oversampling Algorithms**

* **Oversampling** - RandomOverSampler
  * Balanced Accuracy Score: 63.4%
  * Precision: 99%
  * Recall: 68%
 
![Balanced Accuracy Score - OverSampling](https://user-images.githubusercontent.com/75765653/114323231-e41b8b80-9ae9-11eb-9a0a-9f51dd9331ff.PNG)
![Classification Report - OverSampling](https://user-images.githubusercontent.com/75765653/114323225-e382f500-9ae9-11eb-85a2-ebcef3d88190.PNG)

* **Oversampling** - SMOTE
  * Balanced Accuracy Score: 64.7%
  * Precision: 99%
  * Recall: 63%

![Balanced Accuracy Score - SMOTE](https://user-images.githubusercontent.com/75765653/114323232-e41b8b80-9ae9-11eb-958a-ef480662ebf1.PNG)
![Classification Report - SMOTE](https://user-images.githubusercontent.com/75765653/114323226-e382f500-9ae9-11eb-9613-b5461cfa930a.PNG)

* **Undersampling** - ClusterCentroids 
  * Balanced Accuracy Score: 64.7%
  * Precision: 99%
  * Recall: 45%

![Balanced Accuracy Score - Undersampling](https://user-images.githubusercontent.com/75765653/114323233-e4b42200-9ae9-11eb-984c-45ef71353689.PNG)
![Classification Report - Undersampling](https://user-images.githubusercontent.com/75765653/114323227-e382f500-9ae9-11eb-9b04-076a10adaf75.PNG)

* **CombinationSampling** - SMOTEENN
  * Balanced Accuracy Score: 52.9%
  * Precision: 99%
  * Recall: 57%

![Balanced Accuracy Score - Combo](https://user-images.githubusercontent.com/75765653/114323229-e41b8b80-9ae9-11eb-9eb2-84498a05970f.PNG)
![Classification Report - Combo](https://user-images.githubusercontent.com/75765653/114323223-e382f500-9ae9-11eb-8e5a-538fcdabb066.PNG)

* **Ensemble Algorithm** - RandomForestClassifer
  * Balanced Accuracy Score: 78.8%
  * Precision: 99%
  * Recall: 91%

![Balanced Accuracy Score - Ensemble](https://user-images.githubusercontent.com/75765653/114323230-e41b8b80-9ae9-11eb-9009-955a23343917.PNG)
![Classification Report - Ensemble](https://user-images.githubusercontent.com/75765653/114323224-e382f500-9ae9-11eb-8c4f-8b7bb090ecfc.PNG)

* **Ensemble Algorithm** - EasyEnsembleClassifer
  * Balanced Accuracy Score: 94.3%
  * Precision: 99%
  * Recall: 94%

![Easy Ensemble](https://user-images.githubusercontent.com/75765653/114323228-e41b8b80-9ae9-11eb-91e3-8540af803acf.PNG)

## Summary 
Overall the data does not seem to useful in predicting if a credit card applicant is high risk. All of the sampling models had weak accuracy and recall scores. The Ensemble learning methods hade defnite improvement and I would use these models to predict the credit card applicants risk level. However, the Easy Ensemble model would still predict many applicants as high risk when they are actually low risk, therefore, I would not recommend using any of these algorithms to determine credit risk.

