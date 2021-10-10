# Credit_Risk_Analysis

## Analysis Overview

The purpose of this project is to apply supervised machine learning alogthrims to determine credit card risk. It is in the best interest of financial institutions, banks, and peer-to-peer lending firms to automate and improve the accuracy of detecting high-risk individuals, prior to granting loans to assure minimal default. With machine learning, it is particullary challenging due to imbalanced distribution of risk classification (low risk vs high risk), as in a given sample dataset, there are substanitally more low-risk applicants than low-risk.

To due to the difficulty of screening for fewer high-risk applicants, it is beneficial to deploy various ML models, that reduce bias and resample datasets to determine the best methodology or alogothrim to accurately predict credt-card risk. We adopted the following procedure:

a. oversample the data using the RandomOverSampler and SMOTE algorithms.

b. Undersample the data using the ClusterCentroids algorithm.

c. Use a combinatorial approach of over- and undersampling using the SMOTEENN algorithm.

d. Compare two machine learning models that reduce bias, BalancedRandomForestClassifier and EasyEnsembleClassifier.

## Challenge Deliverables

a. Deliverable 1: Use Resampling Models to Predict Credit Risk

b. Deliverable 2: Use the SMOTEENN Algorithm to Predict Credit Risk

c. Deliverable 3: Use Ensemble Classifiers to Predict Credit Risk

d. Deliverable 4: A Written Report on the Credit Risk Analysis (README.md)

## Results

![1.Naive_Random_Sampling.png](https://github.com/Shikharbhd/Credit_Risk_Analysis/blob/main/Resources/Images/1.Naive_Random_Sampling.png)
The balanced accuracy score is 65%.
The high_risk precision is about 1% only with 67% sensitivity which makes a F1 of 2% only.
Due to the high number of the low_risk population, its precision is almost 100% with a sensitivity of 64%.
![2.SMOTE_OverSampling.png](https://github.com/Shikharbhd/Credit_Risk_Analysis/blob/main/Resources/Images/2.SMOTE_OverSampling.png)
The results are pretty similar to the previous model.
The balanced accuracy score is 63%.
The high_risk precision is about 1% only with 61% sensitivity which makes a F1 of 2% only.
Due to the high number of the low_risk population, its precision is almost 100% with a sensitivity of 64%.
![3.CC_Undersampling.png](https://github.com/Shikharbhd/Credit_Risk_Analysis/blob/main/Resources/Images/3.CC_Undersampling.png)
Here the balanced accuracy score is down to about 63%.
The high_risk precision is still 1% only with 61% sensitivity which makes a F1 of 2%.
The low_risk sensitivity is only 64%.
![4.SMOTEENN_Combination_Sampling](https://github.com/Shikharbhd/Credit_Risk_Analysis/blob/main/Resources/Images/4.SMOTEENN_Combination_Sampling.png)
The balanced accuracy score is about 62%.
The high_risk precision is still 1% only with 71% sensitivity which makes a F1 of only 2%.
Due to the high number of false positives, the low_risk sensitivity is 54%.
![5.BRF_Classifieer](https://github.com/Shikharbhd/Credit_Risk_Analysis/blob/main/Resources/Images/5.BRF_Classifieer.png)
The balanced accuracy score improved to about 79%.
The high_risk precision is still low at 4% only with 67% sensitivity which makes a F1 of only 7%.
Due to a lower number of false positives, the low_risk sensitivity is now 91% with 100% presicion.
![6.EE_Classifieer](https://github.com/Shikharbhd/Credit_Risk_Analysis/blob/main/Resources/Images/6.EE_Classifieer.png)


## Summary
All the models used to perform the credit risk analysis show weak precision in determining if a credit risk is high.
The Ensemble models brought a lot more improvment specially on the sensitivity of the high risk credits.
For those reasons I would not recommend the bank to use any of these models to predict credit risk.
