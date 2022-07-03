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

![Balanced Random Forrest Classifier](https://user-images.githubusercontent.com/100163289/177046674-4014a596-28af-4c2f-8740-b90345226716.png)


Balanced Accuracy: .77

Precision:
  low risk: 1
  high risk: .03
  
Recall:
  low risk: .88
  high risk: .68

### Easy Ensemble AdaBoost ClassifierBalanced Accuracy: 

![AdaBoost Classifier](https://user-images.githubusercontent.com/100163289/177053034-58dd3775-8ba5-40f6-816f-1ac829a512af.png)

Balanced Accuracy: .93

Precision:
  low risk: 1
  high risk: .07
  
Recall:
  low risk: .94
  high risk: .91

## Summary: 
Each of these models show the dangers of over-fitting or under-fitting the data and the importance of testing the data to ensure you get reliable results for your analysis. When determining the risk of default for particular customers, it is safe to assume that the number of customers who have not defaulted are vastly larger than those that have. In this instance, the AdaBoost Classifier is the best model to use as it provides the highest Balance Accuracy score. The least reliable model would be the Under-sampling model that returned Balance Accuracy  score of .51. 

Additionally, the AdaBoost Classifier model has a better Precision Score than the other models. The Random Forrest is the only other model that does not have a high risk of .01 and low risk of 1. This means that every model caught 100% of the low-risk borrowers, but did a pretty poor job of identifying 100% of the high-risk borrowers. This is a common risk when you are training a model to identify a small subset of individuals within a much larger data set. You should probably scale the high-risk borrowers so they are over represented in the testing phase so your model has more exposure to them. This will result in a better model that is better able to better identify high-risk borrowers. 


