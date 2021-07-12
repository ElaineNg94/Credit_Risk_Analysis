# Credit_Risk_Analysis
## Overview of the loan prediction risk analysis:
The purpose of this analysis was to help the lead data scientist, Jill to predict credit risk at her company. I had to build and evaluate several machine learning models or algorithms to see which model would be best at predicting credit risk. I used techniques like resampling and boosting for these models and my data. Then I had to evaluate each model’s performance to see how well each one predicts data, since machine learning is good at helping businesses like banks and financial institutions predict anomalies, reduce risk cases, monitor portfolios, and provide recommendations on what to do in cases of fraud. 

## Results:

### Naive Random Oversampling

- #### Balanced Accuracy Score:
<img width="723" alt="Naive Random Oversampling balanced accuracy" src="https://user-images.githubusercontent.com/79742633/125186100-39e0fc00-e1dd-11eb-9d95-dd267a5f608b.png">

- #### Confusion Matrix:
<img width="701" alt="Naive Random Oversampling confusion matrix" src="https://user-images.githubusercontent.com/79742633/125185894-284b2480-e1dc-11eb-82d2-f4870a6eb8cf.png">

- #### Imbalanced Classification Report:
<img width="702" alt="Naive Random Oversampling imbalanced classification report" src="https://user-images.githubusercontent.com/79742633/125185893-27b28e00-e1dc-11eb-9632-e799c23ee3b5.png">

From these pictures shown above, when using **Naive Random Oversampling** the balanced accuracy score is 0.6603423204808787. The precision score was 0.99 and the recall score was 0.58.

### SMOTE Oversampling

- #### Balanced Accuracy Score:
<img width="726" alt="SMOTE Oversampling balanced accuracy" src="https://user-images.githubusercontent.com/79742633/125192203-71f73780-e1fb-11eb-9333-b185d851eb18.png">

- #### Confusion Matrix:
<img width="726" alt="SMOTE Oversampling confusion matrix" src="https://user-images.githubusercontent.com/79742633/125192205-71f73780-e1fb-11eb-8691-4e610624b7ef.png">

- #### Imbalanced Classification Report:
<img width="720" alt="SMOTE Oversampling imbalanced classification report" src="https://user-images.githubusercontent.com/79742633/125192198-70c60a80-e1fb-11eb-9f39-0d7e30952f1d.png">

From these pictures shown above, when using **SMOTE Oversampling** the balanced accuracy score is 0.6537310478007576. The precision score was 0.99 and the recall score was 0.68.

### ClusterCentroids Undersampling

- #### Balanced Accuracy Score:
<img width="720" alt="ClusterCentroids Undersampling balanced accuracy" src="https://user-images.githubusercontent.com/79742633/125192192-660b7580-e1fb-11eb-89ed-daec65183a6b.png">

- #### Confusion Matrix:
<img width="720" alt="ClusterCentroids Undersampling confusion matrix" src="https://user-images.githubusercontent.com/79742633/125192191-660b7580-e1fb-11eb-8168-0da73cc1b339.png">

- #### Imbalanced Classification Report:
<img width="718" alt="ClusterCentroids Undersampling classification report" src="https://user-images.githubusercontent.com/79742633/125192190-6572df00-e1fb-11eb-9d94-fbe21236146e.png">

From these pictures shown above, when using **ClusterCentroids Undersampling** the balanced accuracy score is 0.5447046721744204. The precision score was 0.99 and the recall score was 0.40.

### SMOTEENN Combination Sampling

- #### Balanced Accuracy Score:
<img width="725" alt="SMOTEENN Combination sampling balanced accuracy" src="https://user-images.githubusercontent.com/79742633/125192199-715ea100-e1fb-11eb-8156-666b4bfb9f17.png">

- #### Confusion Matrix:
<img width="725" alt="SMOTEENN Combination sampling confusion matrix" src="https://user-images.githubusercontent.com/79742633/125192202-715ea100-e1fb-11eb-92d0-103245b3ec92.png">

- #### Imbalanced Classification Report:
<img width="721" alt="SMOTEENN Combination sampling classification report" src="https://user-images.githubusercontent.com/79742633/125192200-715ea100-e1fb-11eb-8315-14c6c513302b.png">

From these pictures shown above, when using **SMOTEENN Combination Sampling** the balanced accuracy score is 0.6447993752836463. The precision score was 0.99 and the recall score was 0.57.

### Balanced Random Forest Classifier

- #### Balanced Accuracy Score:
<img width="728" alt="balanced random forest balanced accuracy" src="https://user-images.githubusercontent.com/79742633/125234611-e8487800-e295-11eb-947b-aa1bc3b2952f.png">

- #### Confusion Matrix:
<img width="728" alt="balanced random forest confusion matrix" src="https://user-images.githubusercontent.com/79742633/125234612-e8487800-e295-11eb-89d2-bfc3a72f67fe.png">

- #### Imbalanced Classification Report:
<img width="726" alt="balanced random forest imbalanced classification" src="https://user-images.githubusercontent.com/79742633/125234613-e8e10e80-e295-11eb-9804-c1444451f9ee.png">

From these pictures shown above, when using **Balanced Random Forest Classifier** the balanced accuracy score is 0.7885466545953005. The precision score was 0.99 and the recall score was 0.87.

### Easy Ensemble AdaBoost Classifier

- #### Balanced Accuracy Score:
<img width="727" alt="easy ensemble balanced accuracy" src="https://user-images.githubusercontent.com/79742633/125234635-eed6ef80-e295-11eb-862a-83e3a5c3eecf.png">

- #### Confusion Matrix:
<img width="727" alt="easy ensemble confusion matrix" src="https://user-images.githubusercontent.com/79742633/125234630-ee3e5900-e295-11eb-8de7-647beae509f7.png">

- #### Imbalanced Classification Report:
<img width="728" alt="easy ensemble imbalanced classification" src="https://user-images.githubusercontent.com/79742633/125234632-ee3e5900-e295-11eb-93f5-b3b21b02ba2a.png">

From these pictures shown above, when using **Easy Ensemble AdaBoost Classifier** the balanced accuracy score is 0.9316600714093861. The precision score was 0.99 and the recall score was 0.94.

## Summary:
When looking at these six different models, I noticed that all of these models came out with the same precision score of 0.99, but different recall scores. These six analysis also showed that all of them are more sensitive than precise, which that can be good when detecting credit risk because it can detect more fraud and see if it actually is fraud. We also looked at the balanced accuracy score of each model. **ClusterCentroids Undersampling** had the lowest balanced accuracy score and lowest recall score compared to the rest of the models, so I wouldn’t recommend the ClusterCentroids Undersampling model to predict credit risk. The ClusterCentroids model was also the only model that used undersampling. That can show that undersampling is not good when detecting credit risk. I would recommend the **EasyEnsembleClassifier** method because it had the highest balanced accuracy score and highest recall score out of the rest of these models, which means it can be good at detecting credit risk.
