# Exploratory-Data-Analysis

This repository consists of the code used for performing the Exploratory Data Analysis.

YouTube Link : https://www.youtube.com/watch?v=ZVN-g1MbK-c&t=56s

App Link : https://exploratory-data-analysis--app.herokuapp.com/


The dataset consists of 1042 rows and 20 columns. This is a regression problem where we
can the target variable is 'price' which I have predicted using Machine Learning Modeling.
I Dropped the columns 'id', 'time_created','time_updated','external_id','url','latitude' and
'longitude' from the dataset, as these variables do not provide information significant in
modeling.
I have observed that the variable 'status' has only one value throughout the dataset i.e.
'active', hence I have can drop this variable as it is not providing us significant information.
I observed that the variables 'bedrooms' ,'bathrooms', 'garages' ,'parkings' ,'offering' ,'erf_size' ,'
floor_size' have missing values and the target variable 'price' also has missing values. Hence I
took care of this by filling the missing values of the independent features and the target
variable.
After making the above observation I filled the two rows which have value '[None]' in the
property_type column with 'house' as the value for the'agency' variable for these rows is
'rawson' and the mode for the variable 'property_type' for the agency 'rawson' is 'house' and
also mode for the 'property_type' variable for the area 'Constantia' is also 'house'
I also predicted the missing Values Using Imputers From sklearn.preprocessing
I have also used the KNNImputer to fill the missing values in the variables 'price',
"garages","parkings","erf_size","floor_size" by predicting the values using the KNNImputer
library.
