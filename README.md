# credit_risk_analysis
# Module 17: Supervised Machine Learning and Credit Risk

## Overview of the loan prediction risk analysis:
Credit risk is an inherently unbalanced classification problem, as good loans easily outnumber risky loans. Therefore, one needs to employ different techniques to train and evaluate models with unbalanced classes. We will use imbalanced-learn and scikit-learn libraries to build and evaluate models using resampling.

Using the credit card credit dataset from LendingClub, a peer-to-peer lending services company, we’ll oversample the data using the RandomOverSampler and SMOTE algorithms, and undersample the data using the ClusterCentroids algorithm. Then, we’ll use a combinatorial approach of over- and undersampling using the SMOTEENN algorithm. Next, we’ll compare two new machine learning models that reduce bias, BalancedRandomForestClassifier and EasyEnsembleClassifier, to predict credit risk. Then, we’ll evaluate the performance of these models and make a written recommendation on whether they should be used to predict credit risk.

### Deliverable 1: Use Resampling Models to Predict Credit Risk
For all three algorithms, the following have been completed:
- An accuracy score for the model is calculated
- A confusion matrix has been generated
- An imbalanced classification report has been generated

### Deliverable 2: Use the SMOTEENN Algorithm to Predict Credit Risk
The combinatorial SMOTEENN algorithm does the following:
- An accuracy score for the model is calculated
- A confusion matrix has been generated
- An imbalanced classification report has been generated

### Deliverable 3: Use Ensemble Classifiers to Predict Credit Risk
The BalancedRandomForestClassifier algorithm does the following:
- An accuracy score for the model is calculated
- A confusion matrix has been generated
- An imbalanced classification report has been generated
- The features are sorted in descending order by feature importance

The EasyEnsembleClassifier algorithm does the following:
- An accuracy score of the model is calculated
- A confusion matrix has been generated
- An imbalanced classification report has been generated


## Results: 
Here is a bulleted list that describes the balanced accuracy score and the precision and recall scores of all six machine learning models

1.	Oversampling
•	Naïve Random Oversampling

![fig1_Naive_Random_Oversampling_Accuracy_Score](https://github.com/veenapu/credit_risk_analysis/blob/main/Images/fig1_Naive_Random_Oversampling_Accuracy_Score.PNG)

![fig2_Naive_Random_Oversampling_Precision](https://github.com/veenapu/credit_risk_analysis/blob/main/Images/fig2_Naive_Random_Oversampling_Precision_%26_Recall_Scores.PNG)

- Balanced Accuracy Score is 66%
- High Risk precision is about 1% and a sensitivity of 63% which gives F1 a mere 2%
- Due to high number of low risk population, the precision is 100% with a sensitivity of about 69%.

•	SMOTE Oversampling

![fig3_SMOTE_Oversampling_Accuracy_Score](https://github.com/veenapu/credit_risk_analysis/blob/main/Images/fig3_SMOTE_Oversampling_Accuracy_Score.PNG)

![fig4_SMOTE_Oversampling_Precision_%26_Recall_Scores](https://github.com/veenapu/credit_risk_analysis/blob/main/Images/fig4_SMOTE_Oversampling_Precision_%26_Recall_Scores.PNG)

- Balanced Accuracy Score is 66%
- High Risk precision is about 1% and a sensitivity of 69% which gives F1 a mere 2%
- Due to high number of low risk population, the precision is 100% with a sensitivity of about 63%.

2.	Under Sampling

![fig5_Undersamplig_Accuracy_Score](https://github.com/veenapu/credit_risk_analysis/blob/main/Images/fig5_Undersamplig_Accuracy_Score.PNG)

![fig6_Undersamplig_Precision_&_Recall_Scores](https://github.com/veenapu/credit_risk_analysis/blob/main/Images/fig6_Undersamplig_Precision_%26_Recall_Scores.PNG)

- Balanced Accuracy Score is 54%
- High Risk precision is about 1% and a sensitivity of 40% which gives F1 a mere 1%
- Due to high number of low risk population, the precision is 100% with a sensitivity of about 69%.

3.	Combination Sampling (Over and Under)

![fig7_Combination_Sampling_Accuracy_Score](https://github.com/veenapu/credit_risk_analysis/blob/main/Images/fig7_Combination_Sampling_Accuracy_Score.PNG)

![fig8_Combination_Sampling_Precision_&_Recall_Scores](https://github.com/veenapu/credit_risk_analysis/blob/main/Images/fig8_Combination_Sampling_Precision_%26_Recall_Scores.PNG)

- Balanced Accuracy Score is 64%
- High Risk precision is about 1% and a sensitivity of 57% which gives F1 a mere 2%
- Due to high number of low risk population, the precision is 100% with a sensitivity of about 72%.

4.	Ensemble Learners
•	Balanced Random Forest Classifier

![fig9_Balanced_Random_Forest_Classifier_Accuracy_Score](https://github.com/veenapu/credit_risk_analysis/blob/main/Images/fig9_Balanced_Random_Forest_Classifier_Accuracy_Score.PNG)

![fig10_Balanced_Random_Forest_Classifier_Precision_&_Recall_Scores](https://github.com/veenapu/credit_risk_analysis/blob/main/Images/fig10_Balanced_Random_Forest_Classifier_Precision_%26_Recall_Scores.PNG)

- Balanced Accuracy Score is 79%
- High Risk precision is about 3% and a sensitivity of 87% which gives F1 of 6%
- Due to high number of low risk population, the precision is 100% with a sensitivity of about 70%

•	Easy Ensemble AdaBoost Classifier

![fig11_Easy_Ensemble_Adaboost_Classifier_Accuracy_Score](https://github.com/veenapu/credit_risk_analysis/blob/main/Images/fig11_Easy_Ensemble_Adaboost_Classifier_Accuracy_Score.PNG)

![fig12_Easy_Ensemble_Adaboost_Classifier_Precision_&_Recall_Scores_](https://courses.bootcampspot.com/courses/1559/assignments/30079?module_item_id=597082)

- Balanced Accuracy Score is 93%
- High Risk precision is about 9% and a sensitivity of 94% which gives F1 of 16%
- Due to high number of low risk population, the precision is 100% with a sensitivity of about 92%

## Summary: 
- Summarize the results of the machine learning models, and 
- include a recommendation on the model to use, if any. If you do not recommend any of the models, justify your reasoning.

Compared to all six models, the Easy Ensemble AdaBoost Classifier model yielded the best results with an Accuracy Score of 93.2% and a Precision Rate of 9% for the High Risk applicants. The Recall/Sensitivity rate is also the highest at 92% when compared to all models. For Low Risk applicants, the Recall/Sensitivity rate is also the highest – 94% with a F1 Score of 97%. So, this model would be an ideal model to be recommended to perform this kind of analysis.

### Ranking of models in descending order based on “High Risks” results:
1)	Easy Ensemble AdaBoost Classifier
Accuracy – 93.2%, Precision – 9%, Recall – 92%, F1 – 16%

2)	Balanced Random Forest Classifier
Accuracy – 78.9%, Precision – 3%, Recall – 70%, F1 – 6%

3)	SMOTE Oversampling
Accuracy – 66.2%, Precision – 1%, Recall – 63%, F1 – 2%

4)	Naïve Random Oversampling
Accuracy – 66.0%, Precision – 1%, Recall – 69%, F1 – 2%

5)	Combination Sampling (Over and Under)
Accuracy – 64.5%, Precision – 1%, Recall – 72%, F1 – 2%

6)	Under Sampling
Accuracy – 54.5%, Precision – 1%, Recall – 69%, F1 – 2%



