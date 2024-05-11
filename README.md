# housepriceprediction
Banglore_house_price_prediction:
Creating a machine learning for predicting Banglore house price prediction leveraging a linear regression model to fit the data and the train the model
Data set link:
https://www.kaggle.com/datasets/bandhansingh/banglore-house-price-data
The data set contains attributes like 'location',' total_sqft', 'bath' , 'bhk'
 Data Cleaning: Handling NA values
 Add new feature(integer) for bhk (Bedrooms Hall Kitchen)
 The total_sqft can be a range (e.g. 2100-2850). For such case we can just take average of min and max value in the range. 
 We need to apply dimensionality reduction techniques  to reduce number of locations
 Dimensionality Reduction:
Any location having less than 10 data points should be tagged as "other" location. This way number of categories can be reduced by huge amount. Later on when we do one hot encoding, it will help us with having fewer dummy columns
Outlier Removal Using Business Logic:
1.Outlier Removal Using Standard Deviation and Mean
Model Building:
1.Using K Fold cross validation to measure accuracy of our LinearRegression model
2.Find best model using GridSearchCV
