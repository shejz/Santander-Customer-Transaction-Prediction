# [Santander Customer Transaction Prediction](https://www.kaggle.com/c/santander-customer-transaction-prediction)

The purpose of this competition is to provide a classification model for Santander bank in order to determine which customer will make a specific transaction in the future using an untagged dataset of 200 features and 200,000 training observations.


## **Data**
- The data is anonymous with no customer details been revealed to the participants of the competition.
- Training data set containing **200,000** observations with **200** numeric feature variables and a string `ID_code` column and the binary `target` column which are the outcome of the transaction.   
- The same columns are present for test data except for the `target` as this column we have to predict using the train data set.

## **Exploratory Data Analysis**
Exploratory data analysis mainly includes **missing value**, **outlier**, **correlation**, **descriptive** and visualizations to gain insights from data.

#### Missing Value
- There were no missing values in both train and test data.

#### Imbalanced Dataset
- The dataset is highly imbalanced where only **10%** of the training datais tagged as **1** in the variable target which is an indicator flagging whether if a customer made a transaction. This is important feature to keep in mind as we may need to oversample the customers that made transaction to create a better model.

A bar chart showing the imbalanced distribution in the training data can be seen below:
![Target Distribution](https://github.com/shejz/Santander-Customer-Transaction-Prediction/blob/master/graphs/target_distribution.jpg)

#### Correlation Analysis
- As from the heatmap, variables in train and test data are independent of each other.
![Correlations](https://github.com/shejz/Santander-Customer-Transaction-Prediction/blob/master/graphs/correlations.jpg)
 
## **Preprocessing**
1. Removing fake/synthetic samples in the test set.
2. Count Encoding
3. Combination of extracted training set and real samples as features.

## **Submission and LB Score**

|Model|Public score|Private score|Final rank| 
|------|-------|-------|-------------|
| LGBM |0.98122|0.98206| 223th ( 1309/8802[Top 15%](https://www.kaggle.com/shielaj/competitions))|
| Modified LGBM |0.98122|0.98206| |
| CNN |0.98122|0.98206| |


