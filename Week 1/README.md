# Name: Avadhoot Gorakh Jadhav

## Task 1
* Firstly, to convert categorical variables from column 'Species'; LabelEncoder function from sklearn library is used.
* The model used is xgboost model as it works well for small to medium dataset.
* The calculate_training_loss function takes size of training data partition as inout and calculate the value of loss function "mlogloss" {for multi-class classification} for both training and testing dataset.
* After varying input (training partition size) as 0.5, 0.55, 0.6 ....0.9 the minimum test loss obtained was at partition 0.8 : 0.2

## Task 2
* Firstly, the percentage of missing values in every column was calculated and columns which have very high percentage of missing values were dropped.
* Then the columns containing info which won't affect the outcome were also dropped
* For filling missing values in 'age' column median imputation is used.
* From the remaining data, categorical variable are converted to numeric, again using LabelEncoder function.
* All the columns are scaled using standardscaler.
* After the data was processed, The dataset was trained using KNN classifier, naive-bayes classifier and decision tree and xgboost. Then for each classifier tuning of the parameters was done to find out the best values of parameter. The final accuracy obtained for each model is as follows: 


<center>

| Classifier | Accuracy |
| ---------- | ------- |
| KNN | 86.1% |
| naive-bayes | 83.86% |
| decision tree  |  79.82%  |
| xgboost  | 83.86% |

</center>
  
  
  
##Submission Result
---
**• Submission Accepted** </br>
**• Assignment 2:** https://drive.google.com/file/d/1aQ62-UioJ5y-aKBXhk5TutvDl7uhv-ZW/view?usp=sharing

