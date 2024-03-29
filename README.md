# Retail-Analytics-
The following project uses the sales data to answer the following questions
* How should we allocate our limited marketing budget for next year?
* What type on influencers should we focus on?
* Can we cut budget from TV, as it is too expensive?
* Finally, set your assumptions of the marketing budget and influencer (if any). Can you try to predict the expected sales based on the best ML model?

## Flow of the project 

### Data Cleaning
Identified various categorical and continuous datasets, created dummy variables for the <b>categorical</b> data and filling in the missing values for the <b>continuous</b> data

### Splitting Data
Using test train and split to split the data into 3 parts i.e. train, test and validation set

### Analysis 
Applied the following algorithms and trained them on the training dataset using <b>k folds cross validation</b>
* Linera Regression
* Random Forest Regressor
* Decision tree Regressor 
* Support Vector Regressor 
* Polynomial Regressor 

Used joblib pickled the various hyperparameter settings of the algorithms and saved it in a <b>Model dictionary</b> used and then tested it on the validation dataset

![image](https://user-images.githubusercontent.com/69895829/124377191-50acbd80-dcc8-11eb-9f10-66a2c443a950.png)


Crated a class to analyse the mean squared error and r-squared values that checked the latency of the various models used
![image](https://user-images.githubusercontent.com/69895829/124377165-3246c200-dcc8-11eb-8e8c-189c82674983.png)

After the validation it was fount that <b>Random Forest Regressor</b> with <u>max depth of 8 and 250 different decision trees</u> was the best in performance and gave accurate results 
![image](https://user-images.githubusercontent.com/69895829/124377210-79cd4e00-dcc8-11eb-955d-6c9e4fefa22b.png)

