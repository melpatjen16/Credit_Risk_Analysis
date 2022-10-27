# Credit_Risk_Analysis - Lending Club 

## Overview of the analysis: 

Purpose - An examination of credit risk data was performed using different techniques to train and evaluate models with unbalanced classes. Using the credit card credit dataset from LendingClub, a peer-to-peer lending services company, we have:  oversampled the data with RandomOverSampler and SMOTE algorithms; under-sampled the data using the ClusterCentroids algorithm; and utilized the combinatorial approach of over- and under-sampling using the SMOTEENN algorithm. 

Additionally, we introduced two new machine learning models that reduce bias, BalancedRandomForestClassifier and EasyEnsembleClassifier, to predict credit risk.

## Results: 

The following bulleted lists describes the balanced accuracy scores and the precision and recall scores of all six machine learning models. See screenshots to review results, 

1. _RandomOverSampler_ - The results yielded a moderate recall measure for low risk applicants (0.60)  with a high f1 score. Precision for all models remain relatively constant. This should be noted for the remain models. The accuracy for this model was 0.67. 

Table 1. 

![Screen Shot 2022-10-26 at 11 40 41 PM](https://user-images.githubusercontent.com/107972848/198185936-13f8ffc4-09f2-4a07-acde-e5b737fc54a3.png)


2. _SMOTE_ - The classification table presented a similar precision to the above classification, a slightly greater recall and higher f1 score. The accuracy for this model was slightly less than the previous model (0.66). 

Table 2. 

![Screen Shot 2022-10-26 at 11 56 11 PM](https://user-images.githubusercontent.com/107972848/198187743-a3606fe6-e856-497e-84ba-26db6e04c285.png)


3. _ClusterCentroids_ - This model and approach to under-sampling s=results in a significantly lower recall and f1 score. The accuracy remain similar to the Table 2. Considering these results, under-sampling would not be my preferred approach. 

Table 3. 

![Screen Shot 2022-10-27 at 12 01 05 AM](https://user-images.githubusercontent.com/107972848/198188334-5478ef72-db80-4c7f-ab7e-b7674902d717.png)


4. _SMOTEENN_ - The SMOTTEENN method of modeling loan status outcomes that uses over and under sampling. The approach yielded improved recall and f1 scores compared to under sampling alone but resulted in lower accuracy for predicting loan status. 

Table 4. 

![Screen Shot 2022-10-27 at 12 10 19 AM](https://user-images.githubusercontent.com/107972848/198189409-6ad721c7-0c81-4282-a774-66b0ece7b452.png)


5. _BalancedRandomForestClassifier_ - Two new approach to sampling data to obtain a powerful model was BalancedRandomForestClassifier to obtain a good fitting model for the prediction of loan status. As can be seen, the classification table resulted in slight change (oddly) to precision, an improved recall, and a decent f1 score. Accuracy was not diminished in the model (0.78). 

Table 5. 

![Screen Shot 2022-10-27 at 12 16 04 AM](https://user-images.githubusercontent.com/107972848/198190344-8d8aa15e-ff59-4698-9de3-6251ecb21ee9.png)


6. EasyEnsembleClassifier - This classifier training data approach yield the best approach to modeling predicting loan status. All data element of the classification table improved, including accuracy. This give the data scientist caution as it may indicate overfitting, but at this stage, it seems the best fitting model for the ML project. 

Table 6. 

![Screen Shot 2022-10-27 at 12 22 24 AM](https://user-images.githubusercontent.com/107972848/198191112-f1cb5e24-386b-411a-ae7b-adec7dfab4f2.png)



## Summary: 

Overall, the best approach for training the Lending Tree data was the easyEnsembleClassifier approach. Additionally analysis could examine whether this would perform as well for all risk levels. The second option would be RandomOverSampling. in contrast, future tests using the model should not consider undersampling. 

