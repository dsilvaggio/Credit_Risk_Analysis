# Credit_Risk_Analysis
## Overview
Credit card data from LendingClub, a peer-peer lending service company, was used to analyze credit card risk. Using the **imbalanced-learn** and **skikit-learn** libraries, several machine learning models were built and evaluated using resampling. The data was oversampled using **RandomOverSampler** and **SMOTE**, undersampled using **ClusterCentroids**, then a combination approach of both over and undersampling was done using **SMOTEENN**. To reduce bias, **BalancedRandomForestClassifier** and **EasyEnsembleClassifier** were also run and evaluated. The performance of all six models was evaluated on whether or not they should be used to predict credit risk.  
## Results 
### Naive Random Oversampling
![This is an image](https://github.com/dsilvaggio/Credit_Risk_Analysis/blob/main/Resources/Screen%20Shot%202022-06-14%20at%201.25.11%20PM.png)
![This is an image](https://github.com/dsilvaggio/Credit_Risk_Analysis/blob/main/Resources/Screen%20Shot%202022-06-14%20at%201.25.21%20PM.png)
### SMOTE Oversampling
![This is an image](https://github.com/dsilvaggio/Credit_Risk_Analysis/blob/main/Resources/Screen%20Shot%202022-06-14%20at%201.27.20%20PM.png)
![This is an image](https://github.com/dsilvaggio/Credit_Risk_Analysis/blob/main/Resources/Screen%20Shot%202022-06-14%20at%201.27.26%20PM.png)
### Undersampling
![This is an image](https://github.com/dsilvaggio/Credit_Risk_Analysis/blob/main/Resources/Screen%20Shot%202022-06-14%20at%201.28.36%20PM.png)
![This is an image](https://github.com/dsilvaggio/Credit_Risk_Analysis/blob/main/Resources/Screen%20Shot%202022-06-14%20at%201.28.42%20PM.png)
### Combination (Over and Under) Sampling
![This is an image](https://github.com/dsilvaggio/Credit_Risk_Analysis/blob/main/Resources/Screen%20Shot%202022-06-14%20at%201.29.43%20PM.png)
![This is an image](https://github.com/dsilvaggio/Credit_Risk_Analysis/blob/main/Resources/Screen%20Shot%202022-06-14%20at%201.29.48%20PM.png)
### Balanced Random Forest Classifier
![This is an image](https://github.com/dsilvaggio/Credit_Risk_Analysis/blob/main/Resources/Screen%20Shot%202022-06-14%20at%201.30.49%20PM.png)
![This is an image](https://github.com/dsilvaggio/Credit_Risk_Analysis/blob/main/Resources/Screen%20Shot%202022-06-14%20at%201.30.56%20PM.png)
### Easy Ensemble AdaBoost Classifier
![This is an image](https://github.com/dsilvaggio/Credit_Risk_Analysis/blob/main/Resources/Screen%20Shot%202022-06-14%20at%201.32.00%20PM.png)
![This is an image](https://github.com/dsilvaggio/Credit_Risk_Analysis/blob/main/Resources/Screen%20Shot%202022-06-14%20at%201.32.08%20PM.png)
## Summary
