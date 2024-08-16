# **Dynamic-Price-Prediction**

Uber and Lyft's ride prices are not constant like public transport. They are greatly affected by the demand and supply of rides at a given time. 
So what exactly drives this demand? The first guess would be the time of the day; times around 9 am and 5 pm should see the highest surges on account of people commuting to work/home.
Another guess would be the weather; rain/snow should cause more people to take rides.

The data is approx. for a week of Nov '18 ( I actually have included data collected while I was testing the 'querying' application so might have data spread out over more than a week.
I didn't consider this as a time-series problem so did not worry about regular interval. The chosen interval was to query as much as data possible without unnecessary redundancy.
So data can go from end week of Nov to few in Dec) The Cab ride data covers various types of cabs for Uber & Lyft and their price for the given location. 
You can also find if there was any surge in the price during that time. Weather data contains weather attributes like temperature, rain, cloud, etc for all the locations taken into consideration. 
By finding the most related factors that affect fare prices, we will first use XGBoost Regression, LGBM Regression and Gradiant BoostRegressor models to find the most accurate model for prediction. 
Then, we will use feature importance to pinpoint the most important factors that influence price for Uber and Lyft separately.
