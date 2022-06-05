# Machine-learning-predecting-the-houses-price
# How to run??
1. Provide a location of the dataset in these two variables which will hold the value of the test and train dataset as shown in the figure below. 


2. Install all the necessary libraries required to run the code. For example :- pip install pandas

# Basic idea:-
* Extracting the data from a particular location and converting it into a data frame.
* Using linear regression to train the model for predicting the house price and for classification random forest classifier is used as it provides good accuracy.
* Lastly, values will be predicted and the accuracy for random forest classifier and root mean square error for linear regression will be calculated.

# Program description:-
* Importing a few basic libraries in python.
* Now, reading the data from a location and deleting the number feature which is irrelevant for training and predicting the model. 
* In this case, the number feature was irrelevant and was dropped. The X values are the features and are independent and the Y values are dependent on the X values.
* Now, import the linear model from the sklearn library in python and fit the linear regression model on the training data set Xtrain and Ytrain.
* Predicting the house prices for the test data set and storing the values in a variable for later use.
* This variable could be converted into data frame using pandas library and the predicted values could be observed.
* Now, root means square error(RMSE) can be calculated by importing the library mean_square_error from sklearn and by passing predicted and the actual values in the parameters. The RSME value was 8.501.
* In classification, the prices of the house should be classified as expensive or not expensive based on the features of the house and the actual price. Before fitting any classification model a new feature Y (which initially just contains the 0 value) is introduced in the training set which is dependent on the ‘Y house price of unit area’. If the price is greater than 30 then its value will be converted to 1 or else it will be just 0.
* Fit the model on the training set. In this case, a random forest classifier was used as it provides good accuracy.
