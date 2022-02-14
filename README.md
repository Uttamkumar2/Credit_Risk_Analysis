# Credit_Risk_Analysis

This project is to predict credit risk using Machine Learning and it's technique's which help to predict and provide more reliable loan experience for the customers. Machine Leaning techniques is believed to give more acurate identification of good candiates for laon which will lower the default rate.

## Analysis Overview 

Used Python and machine Leaning techniques such as resampling and Boasting using libraries like Panda, imbalanced-learn & Scikit-Learn,  to make the most of the model and data. 

* Oversample the data using the RandomOverSampler and SMOTE algorithms.
* Undersample the data using the ClusterCentroids algorithm
* Then used combinatorial approach of over- and undersampling using the SMOTEENN algorithm.
* Compare two new machine learning models that reduce bias, BalancedRandomForestClassifier and EasyEnsembleClassifier, to predict credit risk.
* Evaluate the performance of these models to give recommendation on whether they should be used to predict credit risk.

## Resources

* Software Python 3.7.11, conda 4.11.0, Microsoft Studio Code 1.64.1
* Data Source : LoanStats_2019Q1.csv

## Results

### Naive Random Oversampling: 
Balance accurancy Score is 62.5%, and hign risk presion is low at 1% and recall is at 60% which makes a F1 of 2% Only. Due to the high number of the low_risk with sensitivity of 65%.

![RandomOverSampling1](https://user-images.githubusercontent.com/91766890/153807333-31410d85-cb52-46ac-8226-88f936173c13.png)
![RandomOverSampling2](https://user-images.githubusercontent.com/91766890/153807343-7e32a761-8f0b-402a-a340-2c2a12c6ced5.png)
![RandomOverSampling3](https://user-images.githubusercontent.com/91766890/153807351-fefd4286-74ba-42ab-b0e3-24c651bdb91c.png)

### SMOTE Oversampling:
The accuracy score is 65%, the precision for the high_risk loans has a low positvity again at 1% and recall is 66% overall.
The results are pretty similar to the previous model.

![smoteOversampling1](https://user-images.githubusercontent.com/91766890/153807713-69ae4348-cde2-436e-9847-573b4ca82a16.png)
![smoteOversampling2](https://user-images.githubusercontent.com/91766890/153807729-0a099990-1c60-4b50-93cd-6af0beb70247.png)
![smoteOversampling3](https://user-images.githubusercontent.com/91766890/153807738-8cfc39d7-c2da-4175-8293-a0e2a2095526.png)

### Undersampling: 
Here the balanced accuracy score is down to about 52%. The high_risk precision is still 1% only with 61% sensitivity which makes a F1 of 1%.
Due to the high number of false positives, the low_risk sensitivity is only 45%.


![ClusterCentrorid1](https://user-images.githubusercontent.com/91766890/153807855-a00f9156-d660-430f-b5c2-958acd91c1a4.png)
![ClusterCentrorid2](https://user-images.githubusercontent.com/91766890/153807874-dd621863-dcf2-4f93-bf51-718c594e1e67.png)
![ClusterCentrorid3](https://user-images.githubusercontent.com/91766890/153807884-7e2ec99b-ba00-45a8-b38e-11435c29c9f9.png)

### Combination (Over and Under) Sampling:

The balanced accuracy score is about 61%. The high_risk precision is still 1% only with 69% sensitivity which makes a F1 of only 2%.
Due to the high number of false positives, the low_risk sensitivity is 54%.

![smoteennmodel1](https://user-images.githubusercontent.com/91766890/153808059-bbf0ee7c-3bdc-4cd2-9192-2e972198c0eb.png)
![smoteennmodel2](https://user-images.githubusercontent.com/91766890/153808072-9c051ebd-4c1e-43fd-9500-c63769a0fbc6.png)
![smoteennmodel3](https://user-images.githubusercontent.com/91766890/153808082-57791153-5a1f-425f-93cd-69ab66029bd7.png)

### Balanced Random Forest Classifier:

the accuracy score is 78.78% the precision is 99% and high risk precision is still low at 4% with 67% of sensitivity which makes f1 to 7%
Due to a lower number of false positives, the low_risk sensitivity is now 91% with 100% presicion.

![BalanceRandomForestClassifier1](https://user-images.githubusercontent.com/91766890/153808208-270ab519-4285-450d-a901-79783ae2c477.png)
![BalanceRandomForestClassifier2](https://user-images.githubusercontent.com/91766890/153808218-34b69384-0e2d-4784-b97d-5ef6f8865d39.png)
![BalanceRandomForestClassifier3](https://user-images.githubusercontent.com/91766890/153808223-91289d86-ed6c-4219-ad12-a5b71f9ab3b5.png)

### Easy Ensemble AdaBoost Classifier:

Now, the balanced accuracy score is high to about 92%. The high_risk precision is still low at 7% only with 91% sensitivity which makes a F1 of only 14%.
Due to a lower number of false positives, the low_risk sensitivity is now 94% with 99% presicion.

![easyensempleClassifier1](https://user-images.githubusercontent.com/91766890/153808586-b84cb91e-d0ae-4a52-8249-e3512f3f0877.png)
![easyensempleClassifier2](https://user-images.githubusercontent.com/91766890/153808615-10bed080-a478-4e69-8cd5-c4697f58d35c.png)
![easyensempleClassifier3](https://user-images.githubusercontent.com/91766890/153808623-fa572a57-75e2-4d14-863d-51ba30af59da.png)

## Summary

Overall, the best model that was generated to predict the unbalanced classification problem of credit risk is the Ensemble AdaBoost Classifier as well as the Balanced Random Forest Classifier due to their high precision, recall, and accuracy scores being near 1 which is what we want in this prediction problem. But I would recommend the Ensemble AdaBoost Classifier due to its higher overall scores for a classification prediction.
