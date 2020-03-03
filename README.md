# [Santander Customer Transaction Prediction](https://www.kaggle.com/c/santander-customer-transaction-prediction)

The purpose of this competition is to provide a classification model for Santander bank in order to determine which customer will make a specific transaction in the future using an untagged dataset of 200 features and 200,000 training observations.


## **Data**
- The data is anonymous with no customer details been revealed to the participants of the competition.
- Training data set containing **200,000** observations with **200** numeric feature variables and a string `ID_code` column and the binary `target` column which are the outcome of the transaction.   
- The same columns are present for test data except for the `target` as this column we have to predict using the train data set.

## **Exploratory Data Analysis**
Exploratory data analysis mainly includes **missing value**, **outlier**, **correlation**, **descriptive** and visualizations to gain insights from data.


### Imbalanced Dataset
- The dataset is highly imbalanced where only **10%** of the training datais tagged as **1** in the variable target which is an indicator flagging whether if a customer made a transaction. This is important feature to keep in mind as we may need to oversample the customers that made transaction to create a better model.  

### Correlation Analysis
![Correlations](link-to-image)
 
