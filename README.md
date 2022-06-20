# Credit_Risk_Analysis
## Overview
Credit card data from LendingClub, a peer-peer lending service company, was used to analyze credit card risk. Using the **imbalanced-learn** and **skikit-learn** libraries, several machine learning models were built and evaluated using resampling. The data was oversampled using **RandomOverSampler** and **SMOTE**, undersampled using **ClusterCentroids**, then a combination approach of both over and undersampling was done using **SMOTEENN**. To reduce bias, **BalancedRandomForestClassifier** and **EasyEnsembleClassifier** were also run and evaluated. The performance of all six models was evaluated on whether or not they should be used to predict credit risk.  
## Results 
### Naive Random Oversampling
![This is an image](https://github.com/dsilvaggio/Credit_Risk_Analysis/blob/main/Resources/Screen%20Shot%202022-06-14%20at%201.25.11%20PM.png)
![This is an image](https://github.com/dsilvaggio/Credit_Risk_Analysis/blob/main/Resources/Screen%20Shot%202022-06-14%20at%201.25.21%20PM.png)

* The Balanced Accuracy Score is 64%.
* The high risk precision score is 0.01, the recall score is 0.61, and the f1 score is 0.02. 
*  The low risk precision score is 1, the recall score is 0.68, and the f1 score is 0.81.
### SMOTE Oversampling
![This is an image](https://github.com/dsilvaggio/Credit_Risk_Analysis/blob/main/Resources/Screen%20Shot%202022-06-14%20at%201.27.20%20PM.png)
![This is an image](https://github.com/dsilvaggio/Credit_Risk_Analysis/blob/main/Resources/Screen%20Shot%202022-06-14%20at%201.27.26%20PM.png)

* The Balanced Accuracy Score is 61%.
* The high risk precision score is 0.01, the recall score is 0.53, and the f1 score is 0.02. 
*  The low risk precision score is 1, the recall score is 0.70, and the f1 score is 0.82.
### Undersampling
![This is an image](https://github.com/dsilvaggio/Credit_Risk_Analysis/blob/main/Resources/Screen%20Shot%202022-06-14%20at%201.28.36%20PM.png)
![This is an image](https://github.com/dsilvaggio/Credit_Risk_Analysis/blob/main/Resources/Screen%20Shot%202022-06-14%20at%201.28.42%20PM.png)

* The Balanced Accuracy Score is 56%.
* The high risk precision score is 0.01, the recall score is 0.65, and the f1 score is 0.01. 
*  The low risk precision score is 1, the recall score is 0.48, and the f1 score is 0.65.
### Combination (Over and Under) Sampling
![This is an image](https://github.com/dsilvaggio/Credit_Risk_Analysis/blob/main/Resources/Screen%20Shot%202022-06-14%20at%201.29.43%20PM.png)
![This is an image](https://github.com/dsilvaggio/Credit_Risk_Analysis/blob/main/Resources/Screen%20Shot%202022-06-14%20at%201.29.48%20PM.png)

* The Balanced Accuracy Score is 66%.
* The high risk precision score is 0.01, the recall score is 0.75, and the f1 score is 0.02. 
*  The low risk precision score is 1, the recall score is 0.56, and the f1 score is 0.72.
### Balanced Random Forest Classifier
![This is an image](https://github.com/dsilvaggio/Credit_Risk_Analysis/blob/main/Resources/Screen%20Shot%202022-06-14%20at%201.30.49%20PM.png)
![This is an image](https://github.com/dsilvaggio/Credit_Risk_Analysis/blob/main/Resources/Screen%20Shot%202022-06-14%20at%201.30.56%20PM.png)

* The Balanced Accuracy Score is 80%.
* The high risk precision score is 0.04, the recall score is 0.70, and the f1 score is 0.07. 
*  The low risk precision score is 1, the recall score is 0.91, and the f1 score is 0.95.
### Easy Ensemble AdaBoost Classifier
![This is an image](https://github.com/dsilvaggio/Credit_Risk_Analysis/blob/main/Resources/Screen%20Shot%202022-06-14%20at%201.32.00%20PM.png)
![This is an image](https://github.com/dsilvaggio/Credit_Risk_Analysis/blob/main/Resources/Screen%20Shot%202022-06-14%20at%201.32.08%20PM.png)

* The Balanced Accuracy Score is 91%.
* The high risk precision score is 0.07, the recall score is 0.89, and the f1 score is 0.13. 
*  The low risk precision score is 1, the recall score is 0.94, and the f1 score is 0.97.
## Summary

Based on the above information, all of the six models used have very low precision when it comes to predicting high credit risk. Thus, all six of these models are unreliable in determining true high credit risk. If a credit score is classified as high credit risk, it is relatively unlikely that they are truly a high credit risk based on the low precision scores. On the other hand, both Classifier models returned high recall scores for high credit risk. The highest recall score came from the Easy Ensemble Classifier (0.89). This means that about 89% of people who are a high credit risk will be correctly classified. Overall, based on the low precision scores for all models I would not recommend any to predict credit risk. It is very likely that a large number of false positives will be returend from all models, which means a large percentage of people will be classified as high risk and rejected for loans when they should in fact be approved.   
