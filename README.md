# credit_risk_analysis

## Project Overview
The purpose of this project is to find the best machine learning model to use with data from lending tree in order to determine credit risk. This wil be done with the following methods.
 - Oversample using RandomOverSampler
 - Oversample using SMOTE
 - Undersample using ClusterCentroids
 - Combination over and undersampling using SMOTEENN

### RandomOverSampler
Using random over sampling we have an accuracy score of 66%
Using the below image we can see the model has a 1% precision rate when it comes to classifying high risk. 
Using the below image we can see the model has a 71% recall rate when it comes to classifying low risk. 


![RandomOversampling](https://user-images.githubusercontent.com/88564212/147715176-1960e027-6ecd-454d-afb4-64d7eff1c4ae.png)

### SMOTE
Using SMOTE we have an accuracy score of 66%
Using the below image we can see the model has a 1% precision rate when it comes to classifying high risk. 
Using the below image we can see the model has a 63% recall rate when it comes to classifying low risk. 

![SMOTE](https://user-images.githubusercontent.com/88564212/147715184-9c11cf1d-dd21-4ecb-8b2d-b19cf962f54e.png)

### ClusterCentroids
Using ClusterCentroids we have an accuracy score of 54%
Using the below image we can see the model has a 1% precision rate when it comes to classifying high risk. 
Using the below image we can see the model has a 69% recall rate when it comes to classifying low risk. 

![ClusterCentroids](https://user-images.githubusercontent.com/88564212/147715313-d8f08934-9825-43b8-a2d8-d5ba9787cb59.png)

### SMOTEENN
Using SMOTEENN we have an accuracy score of 64%
Using the below image we can see the model has a 1% precision rate when it comes to classifying high risk. 
Using the below image we can see the model has a 72% recall rate when it comes to classifying low risk. 

![SMOTEENN](https://user-images.githubusercontent.com/88564212/147715204-167ddfc2-fd69-400f-9a0d-8a342eed3733.png)

### BalancedRandomForestClassifier
Using BalancedRandomForestClassifier we have an accuracy score of 79%
Using the below image we can see the model has a 3% precision rate when it comes to classifying high risk. 
Using the below image we can see the model has a 70% recall rate when it comes to classifying low risk. 

![branfor](https://user-images.githubusercontent.com/88564212/147715208-f9c978d7-8753-487f-96fe-b4ba8bca7ad0.png)

### EasyEnsembleClassifier
Using EasyEnsembleClassifier we have an accuracy score of 93%
Using the below image we can see the model has a 9% precision rate when it comes to classifying high risk. 
Using the below image we can see the model has a 92% recall rate when it comes to classifying low risk. 

![easy](https://user-images.githubusercontent.com/88564212/147715213-c8b39e8d-3e1e-4717-96c8-7d49ce2cbf32.png)

## Summary

All of the above models had a poor precision rate, but the best performing model overall was the Easy Ensemble Classifier. While the precision rate was only 9% when detecting high risk, the recall score for both high and low risk were in the low 90s percentage wise. Even though this model performned best it does not mean that it is a good choice for this bank. 16121 applications were deemed high risk while only 983 actually were. A small margin of error in this manner could be good for the business since it would still be giving out a majority of loans while overall protecting the business. With a margin this large it leads to the bank giving out too few loans and overall missing out on revenue  that would largely guarenteed. 

Taking into account that the best behaving model still performs poorly, it is safe to say that none of the models would be a good fit.
