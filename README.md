# CodeSpaze-Internship-housing-prediction-
Housing Prediction 

Housing Sales prediction
Name: Indrajit Burman
Problem statement: 
Develop a regression model to predict future sales based on historical data of housing. This helps in forecasting and planning for inventory, marketing, and budgeting. Because accurate sales predictions enable better decision making and resource the allocation. 
Approach:
Data preprocessing, cleaning and EDA (Exploratory Data Analysis):
Load the csv file of the housing data and understand the data. There are 545 rows and 13 columns.  In this data there are no missing values and no duplicated values. Then I check the statistics of the data for better understanding. I found there are 7 categorical columns and 6 numeric columns. I use label encoder to transform the categorical columns into binary classification.  Then I Check the correlation of the data and visualizing it through a heatmap. I check the price distribution with a hist plot.  Then I perform a scatterplot to see the relation between the price and area, I found that when area is increasing the price is also increasing. Then I see the count plot of all categorical columns. I cerate price per square foot features and display it through a hist plot. 
Model building: 
1)	Linear Regression:
I use linear regression model because the target variable is price and it is continuous. 
Then I divided the data into two parts the is y (the target variable) and X (all columns except price). After that I scaled the X with standard scaler. I used 80% of the data for training purpose and 20% of the data for testing purpose. I perform the linear regression model and see the predictions of test data. 
For evaluating the model, I check: 
Mean Absolute Error (MAE): 503245.29740989994
Mean Squared Error (MSE): 586676606817.3195
Root Mean Squared Error (RMSE): 765948.1750205555
R-squared (R²): 0.8839314564398744
Then I check the threshold for accuracy of the model it gives Accuracy within 10.0%: 66.05504587155964%.
2)	Random Forest Regressor:
Random Forest can rank the importance of features, helping me identify the most influential factors in predicting house prices.  I also use 80% of the data for training purpose and 20% of the data for testing purpose. I implement the random forest regressor and see the predictions of the model. 
For evaluating the model, I check:
Mean Absolute Error (MAE): 503245.29740989994
Mean Squared Error (MSE): 586676606817.3195
Root Mean Squared Error (RMSE): 765948.1750205555
R-squared (R²): 0.9342128099452656
Then I check the threshold for accuracy of the model it gives Accuracy within 10.0%: 85.3211009174312%
Here I can conclude the random forest regressor gives better results than the linear regression. 

