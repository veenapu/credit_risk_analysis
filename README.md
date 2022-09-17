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
- Using bulleted lists, describe the balanced accuracy scores and the precision and recall scores of all six machine learning models. Use screenshots of your outputs to support your results.

## Summary: 
- Summarize the results of the machine learning models, and 
- include a recommendation on the model to use, if any. If you do not recommend any of the models, justify your reasoning.


![fig1_oversampling_counter](https://github.com/veenapu/credit_risk_analysis/blob/main/Images/fig1_oversampling_counter.PNG)

![fig2_balanced_accuracy_score](https://github.com/veenapu/credit_risk_analysis/blob/main/Images/fig2_balanced_accuracy_score.PNG)

![fig3_precision_rate](https://github.com/veenapu/credit_risk_analysis/blob/main/Images/fig3_precision_rate.PNG)

![fig4_undersampling_counter](https://github.com/veenapu/credit_risk_analysis/blob/main/Images/fig4_undersampling_counter.PNG)

![fig5_balanced_accuracy_score](https://github.com/veenapu/credit_risk_analysis/blob/main/Images/fig5_balanced_accuracy_score.PNG)

![fig6_precision_rate](https://github.com/veenapu/credit_risk_analysis/blob/main/Images/fig6_precision_rate.PNG)

![fig7_SMOTEENN_counter](https://github.com/veenapu/credit_risk_analysis/blob/main/Images/fig7_SMOTEENN_counter.PNG)

![fig8_balanced_accuracy_score](https://github.com/veenapu/credit_risk_analysis/blob/main/Images/fig8_balanced_accuracy_score.PNG)

![fig9_precision_rate](https://github.com/veenapu/credit_risk_analysis/blob/main/Images/fig9_precision_rate.PNG)
