# Credit_Risk_Analysis

## Overview of the analysis: 
The purpose of the analysis is to use several different Machine Learning modules to help assess the credit risk of a data set of Lending Club's customers. This will allow Lending Club to make more informed decisions about who to extend loans to and who is a bad credit risk. This should lower Lending Club’s default rate and increase their profitability. 

We accomplish this task by employing the following strategies:
- Naive Random Sampling
- SMOTE Oversampling
- Under sampling
- Combined Over and Under Sampling
- Balanced Random Forest Classifier
- Easy Ensemble AdaBoost Classifier

I use these models to assess their balanced accuracy, precision, and recall scores. The balanced accuracy score is an averaged recall score taken from each class. The precision is a measure of the model's ability to identify only relevant data points and the recall score is a measure of the model's ability to find a certain percentage of bad borrowers. 

## Results: 

### Naive Random Sampling

![Random Sampling](https://user-images.githubusercontent.com/100163289/177021227-68ffdfee-daf6-417f-8cdb-711ec158e602.png)

Balanced Accuracy: .65

Precision:
  low risk: 1
  high risk: .01
  
Recall:
  low risk: .68
  high risk: .62

### SMOTE Oversampling

![SMOTE](https://user-images.githubusercontent.com/100163289/177021302-2e951d94-60e9-47b3-a793-c70e750d4ab7.png)

Balanced Accuracy: .64

Precision: 
  low risk: 1
  high risk: .01
  
Recall:
  low risk: .66
  high risk: .63

### Under sampling

![Under Sampling](https://user-images.githubusercontent.com/100163289/177021655-ab7fbced-bc22-43a5-bfbf-0a3e4d7dc4f9.png)

Balanced Accuracy: .51

Precision:
  low risk: .01
  high risk: 1
  
Recall:
  low risk: .43
  high risk: .60

### Combined Over and Under Sampling

![Combined over and under sampling](https://user-images.githubusercontent.com/100163289/177021787-b4c6497e-fd00-44d4-a296-f27e7fe76c7f.png)


Balanced Accuracy: .63

Precision:
  low risk: 1
  high risk: .01
  
Recall:
  low risk: .57
  high risk: .70


### Balanced Random Forest Classifier




Balanced Accuracy:

Precision:
  low risk:
  high risk:
  
Recall:
  low risk: 
  high risk: 

### Easy Ensemble AdaBoost ClassifierBalanced Accuracy: 



Balanced Accuracy:

Precision:
  low risk:
  high risk:
  
Recall:
  low risk: 
  high risk: 

## Summary: 
Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. If you do not recommend any of the models, justify your reasoning.
