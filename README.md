# Detection of breast cancer using machine learning  
---
## Introduction

Using various machine learning models to detect if an breast cancer is benign or malginant. This was a binary classification problem which 0 represented the cancer being benign and 1 represented that the cancer was malignant. 


## Models implemented 
Different models were implemented and compared in this project using different machine learning techniques. All models are implemented with and without upsampling techniques. 

### Basic models

* Decision Tree (DT)
* Random Forest (RF)
* Logistic Regression (LR)
* Support Vector Machine (SVM)
* Naive Bayes (NB)
* Deep Neural Network (DNN)
* Artificial Neural Network (ANN) 

### Ensemble Models (Different Combinations)

These models are created using the stacking method to combine sets of basic models and act as input which is use to feed into an Artificial Neural Network model. The following are the different set of combination used.

* SVM + LR
* SVM + LR + RF
* SVM + LR + RF + NB
* SVM + LR + RF + DT
* SVM + LR + NB + DT
* SVM + LR + NB + DT + RF

### Other Models

* Artificial Neural Network + Support Vector Machine (As the neural network final layer)


## Results

Basic Models  | Accuracy                                  
------------- | -------------
Decision Tree | 93.6%
Random Forest | 93.0%
Logistic Regression    | 95.7%
Support Vector Machine    | 98.0%
Naive Bayes    | 84.5%
Deep Neural Network    | 95.0%
Artificial Neural Network    | 92.9%


Ensemble Models  | Accuracy
------------- | -------------
SVM+LR | 96.4%
SVM+LR+RF | 98.2%
SVM+LR+RF+NB    | 98.2%
SVM+LR+RF+DT    | 97.6%
SVM+LR+NB+DT    | 97.6%
SVM+LR+NB+DT+RF    | 98.2%

Other Models  | Accuracy
------------- | -------------
ANN+SVM | 96.4%


## Limitations

* Due to the small sample size of the dataset, overfitting was an issue. Hence, models were over-fitted. Techniques such as K-Fold cross validation and batch size/ epoch in neural network were used to handle overfitting issue.




