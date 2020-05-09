# Supervised Machine Learning

## Project overview

The project aims to support Fast Lending better predict credit risk, it was built different models using machine learning to predict those risks. 

## Summary
To lead to a more accurate identification of good candidates to loans which lead to lower default rates it was built and evaluated several machine learning models to predict credit risk. 
Using an imbalanced dataset, it was able to resample the data and build and evaluate logistic regression classifiers using the resampled data.

When naive random oversampling the data, the results were:
- ![alt text]( https://github.com/DaniGio/ML_Supervised/blob/master/Pic/Naive%20Random%20Oversampling.png)

When SMOTE oversampling the data, the results were:
- ![alt text]( https://github.com/DaniGio/ML_Supervised/blob/master/Pic/SMOTE%20Oversampling.png)


When undersampling the data, the results were:
- ![alt text]( https://github.com/DaniGio/ML_Supervised/blob/master/Pic/Undersampling.png)

When using a combination approach with the SMOTEENN algorithm, the results were:
- ![alt text]( https://github.com/DaniGio/ML_Supervised/blob/master/Pic/SMOTEENN.png)

And two different ensemble classifiers to predict loan risk and evaluate each model:

BalancedRandomForestClassifier :
- ![alt text]( https://github.com/DaniGio/ML_Supervised/blob/master/Pic/Balanced%20Random%20Forest%20Classifier.png)

EasyEnsembleClassifier
- ![alt text]( https://github.com/DaniGio/ML_Supervised/blob/master/Pic/Easy%20Ensemble%20AdaBoost%20Classifier.png)

After analizing the different models it is possible to see that the precision, that supports to understand how reliable a positive classification is, shows only high value to "low risk", meaning that we have good chances to identify the "low risk" correctly. But the precision for "high risk" is very low.
Continuing the analysis, it is possibel to identify the recall value, also known as sensitivity. This measurement allows us to understand the value of the corrects predictions. From the models above, only EasyEnsembleClassifier shows a high value for "High Risk".
The accuracy score between predicted values and actual values are also low for all models. 
To conclude, none of the models were very accurated. It is possible to identify the "low risk" status, but for this exercise it is recommended to have better values for "High Risk"- since those are the ones that we really should be flagging.
