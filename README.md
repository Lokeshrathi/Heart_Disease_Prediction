# Heart_Disease_Prediction Classification Problem

- Data has been imported from [Kaggle](https://www.kaggle.com/ronitf/heart-disease-uci).
- The Dependedent feature is named as 'target'
- The shape is 303 rows and 14 columns.
- Our data has balanced dataset 

![](/Images/h3.png)

## Data Visualisation:
- We visualise the data and represent using seaborn.

![](/Images/h1.png)

![](/Images/h2.png)

## Data Cleaning.
- We check for each feature, the range of each feature and how can we optimise our dataset.
- One method is **Removing outliers using Boxplot**

![](/Images/h4.png)

- Using the correlation method, we find the feature which is least correlated and hence drop it.

![](/Images/h5.png)

## Data Modeling
- We use the package **XGBClassifier from xgboost package for classification**
- **Hyperparameter Tuning** to get the best parameters for our model.

![](/Images/h6.png)

- **Cross Validation** to confirm our data doesnot overfit by using **StratifiedKfold with 5 folds**

- We get a **accuracy_score of 90.0% for our model**

> Note: Accuracy_score is given by (TP+TN)/(TP+TN+FP+FN)

> TP- True Positive | TN- True Negative | FP- False Positive | FN - False Negative
