# Regression--Bike-sharing-demand-prediction
Project Summary -
Currently Rental bikes are introduced in many urban cities for the enhancement of mobility comfort. It is important to make the rental bike available and accessible to the public at the right time as it lessens the waiting time. Eventually, providing the city with a stable supply of rental bikes becomes a major concern. The crucial part is the prediction of bike count required at each hour for the stable supply of rental bikes.

First we import the necessary libraries and look at our data and its characteristics. We have a dataset of 8760 rows and 14 columns with no duplicate/missing data. Next we study the features thoroughly and the data it represents. We first see that the column 'Date' is in 'object' datatype, and we convert it to datetime datatype. Later from the date column, we extract, 'Date', 'month', 'year' and number of week, We drop the date column and we rename columns for convinence.

We ploted various charts and explored usefull insites. Based on our visualizations, we formulate 3 hypothetical statements and perform hypothesis tests. The statements are:

The average bike count in Seoul city at any point of time is greater than 100.

The average temperature in Seoul city at any point is grater than 10 degree Celsius.

The Standard deviation of humdidity in Seoul city is 20.

Furthur, we performed one hot encoding on our categorical features with dropping the first column being true. We found out during visualization that our dependant variable, 'Rented_bike_count' was right skewed, hence to overcome this we applied a squareroot transformation to get a normal distribution. Next we scaled our data using MinMax scaler. Finally we split our data into train and test in 80-20 ratio. The data was ready to fit into a machine learning model, we implemented the various models and calculated the various stastical parameters for the performance

Finally, we see that the bike rental company can deploy a machine learning model that uses Random Forest Regressor to predict the demand for city bikes for a particular hour, which can help the company meet the demand accurately.
