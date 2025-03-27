# Diabetes-analysis


This project is aimed at building a machine learning model to predict whether a person has diabetes based on various health-related features. The model uses a dataset containing information such as age, blood pressure, body mass index (BMI), glucose concentration, and more. The goal is to accurately classify whether an individual has diabetes (class 1) or not (class 0).



## Dataset


We will use [Diabetes dataset](https://www.kaggle.com/uciml/pima-indians-diabetes-database), which have 8 numeric features plus a 0-1 class label.

1. Number of times pregnant (`numPregnant`)
2. Plasma glucose concentration a 2 hours in an oral glucose tolerance test (`glucose`)
3. Diastolic blood pressure (mm Hg) (`bloodPress`)
4. Triceps skin fold thickness (`skinThick`)
5. 2-Hour serum insulin (`insulin`)
6. Body mass index (BMI) (`massIndex`)
7. Diabetes pedigree function (`pedigree`)
8. Age (`age`)


## Target 
The target variable represents whether an individual has diabetes or not:
- 0 :  No diabetes
- 1 :   Diabetes


## Model

**K-Nearest Neighbors (KNN)** algorithm  was used to predict diabetes, with the model being trained on the dataset and evaluated using key performance metrics such as `accuracy`, `precision`, `recall` and `F1-score`. 


## Model Report

```

               precision    recall  f1-score   support

           0       0.76      0.89      0.82        97
           1       0.66      0.44      0.53        48

    accuracy                           0.74       145
   macro avg       0.71      0.66      0.67       145
weighted avg       0.73      0.74      0.72       145


```

## Observations

- The model achieves an accuracy of 74%, but there is an imbalance between the target classes (0 and 1).
- The model performs better at predicting non-diabetic cases (class 0) than diabetic cases (class 1).
