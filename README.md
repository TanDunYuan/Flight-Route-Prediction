# Flight Route Prediction

This is a machine learning (supervised) algorithm which aims to predict the flight route which will be flown by an airplane from one airport to another.

The data used data in this project are from two EUROCONTROL databases: historical flight trajectories from the Demand Data Repository (DDR) and air navigation charges from the Central Route Charges Office (CRCO) database.

The data is processed such that features are suitable to be used as input into a gradient boosting classifier algorithm
1. The routes from all the flights in the datasets was clustered into one of the few representative routes typically flown by planes across the origin-destination airport pairs(OD pairs). 
This is done by performing a K-means clustering on the route length and route charges 
2. Then the flights were segmented according to their parameter. The parameters chosen as input to this algorithm was airline, aircraft type and time of day.
3. A machine learning algorithm was developed and evaluated 
  Training: A gradient boosting classifier was trained to predict to choose a route among the cluster of route as identified in step 1. 7
  Validation: The model was validated using  a validation set approach.
  
The dataset provided in this project is from a historical flight trajectory from GCTS-EGKK OD pair from the DDR.

This project is a demonstration of the capability of machine learning in the field of route prediction.
It is a simplified model of a true route prediction model as the inputs are limited. However it can identify the typical routes flown by certain aircraft of a certain company which can be used to show the company's tradeoff between air navigation charges versus the flight time. 
This project is part of a personal project to understand the mechanics behind machine learning in a real world application. 

