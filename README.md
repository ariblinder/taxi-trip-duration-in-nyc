# Predicting the Duration of a Taxicab Ride in NYC

<img src="https://i.imgur.com/UP4GA4s.jpg"/>

Taxicabs are a very important means of transportation throughout many cities and New York City in particular. This notebook anaylzes data gathered in 2016 and originally published by the NYC Taxi and Limousine Commission (TLC) available [here](https://www1.nyc.gov/site/tlc/about/tlc-trip-record-data.page) and made into a competition posted on [Kaggle](https://www.kaggle.com/c/nyc-taxi-trip-duration/overview) which lasted from 7/2017 to 9/2017. In this notebook I provide various models which come close to the highest scoring entries. The training dataset contained the following fields:


*   `id` - a unique identifier for each trip
*   `vendor_id` - a code indicating the provider associated with the trip record
*   `pickup_datetime` - date and time when the meter was started
*   `dropoff_datetime` - date and time when the meter was stopped 
*   `passenger_count` - the number of passengers in the vehicle (driver entered value)
*   `pickup_longitude` - the longitude where the meter was started
*   `pickup_latitude` - the latitude where the meter was stopped
*   `dropoff_longitude` - the longitude where the meter was started
*   `dropoff_latitude` - the latitude where the meter was stopped
*   `store_and_fwd_flag` - This flag indicated whether the trip record was held in vehicle memory before sending to the vendor because the vehicle did not have a connection to the server: `Y` indicates a store and forward trip; `N`indicates a trip which was not a store and forward trip
*   `trip_duration` - duration of the trip in seconds

The test data set provided by Kaggle contains the same fields except `dropoff_datetime` and `trip_duration`.
This notebook proceeds following the outline:

Download the datasets from Kaggle
Prepare and divide the dataset for training and validation
Create and establish a baseline model
Introduce new features
Create linear models, decision trees, and random forests with various hyperparameters

The notebook can be accessed [here](https://jovian.ai/ariblinder/nyc-taxi-ride-time-prediction-v3)
