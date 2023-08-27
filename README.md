# Bike Sharing Assignment

Building a multiple linear regression model for the prediction of demand for shared bikes

## Table of Contents

- [Problem Statement](#problem-statement)
- [Conclusions](#conclusions)
- [Technologies Used](#technologies-used)

## Problem Statement

A US bike-sharing provider BoomBikes has recently suffered considerable dips in their revenues due to the ongoing Corona pandemic. The company is finding it very difficult to sustain in the current market scenario. So, it has decided to come up with a mindful business plan to be able to accelerate its revenue as soon as the ongoing lockdown comes to an end, and the economy restores to a healthy state.

The company wants to know:

1. Which variables are significant in predicting the demand for shared bikes
2. How well those variables describe the bike demands

## Conclusions

The linear regression model aimed to capture the relationship between the target variable "cnt" and several predictor variables. The model's primary goal was to provide accurate predictions of bike rental counts based on weather conditions, time-related factors, and other relevant features.

- Model Performance
  The final model's performance metrics include a low Mean Squared Error (MSE) of 0.0097 and a Root Mean Squared Error (RMSE) of 0.0985, indicating that the model's predictions are generally close to the actual values.

The R-square values provide insights into the amount of variance in the dependent variable that is explained by the independent variables. The R-square of 0.836 for the training set and 0.795 for the testing set suggest that around 83.6% and 79.5% of the variance in 'cnt' is explained by the predictors included in the model, respectively.

The Adjusted R-square values take into account the number of features and the complexity of the model. The Adjusted R-square of 0.832 for the training set and 0.785 for the testing set show that the model retains its explanatory power even after accounting for the number of features.

Hence, this is a good model demonstrating reasonably good fit to the data

- Features Importance
  As per our final model, top 3 features that are significant in predicting demand for shared bikes are:

1. Temperature (temp) : One unit increase in temp variable increases the bike rental count by 0.5636 units. Higher temperatures are associated with higher bike rental counts.

2. Weather (weathersit 3: weather_3_showers) : Compared to reference category weathersit 1, one unit increase in weathersit 3 variable decreases bike rental count by 0.288 units. Presence of showers (weathersit 3) is associated with lower bike rental counts.

3. Year (yr) : One unit increase in year variable increases the bike rental count by 0.233 units. Bike rental counts have increased over the years.

Impact of other predictors are as below:

4. Wind Speed (windspeed) : One unit increase in windspeed variable decreases bike rental count by 0.155 units. Higher wind speeds are more challenging and leads to lower bike rentals.

5. Winter Season (season_winter) : Compared to reference category Season 1 Spring, one unit increase in season 4 i.e., winter variable increases bike rental count by 0.131 units. Might be due to favourable weather conditions in some parts during winter.

6. September (mnth_9) : Compared to reference category Jan, one unit increase in September, mnth_9 increases bike rental count by 0.097 units

7. Summer Season (season_summer) : Compared to reference category Season 1 Spring, one unit increase in season 2 i.e., Summer variable increases bike rental count by 0.087 units. Summer is generally favourable for outdoor activities.

8. Weather (weathersit 2: weather_2_hazy) : Compared to reference category weathersit 1, one unit increase in weathersit 2 variable decreases bike rental count by 0.08 units. Presence of mist and clouds (weathersit 2) is associated with lower bike rental counts.

9. Weekday 6 (day_6) : Compared to reference category Weekday 0 i.e, Sunday, one unit increase in weekday 6 variable increases bike rental count by 0.067 units. Generally people tend to go out on weekends, that explains the increase.

10. Working day (workingday) : One unit increase in workingday variable increases the bike rental count by 0.056 units. More people use bikes to go to office on working days.

11. const : When no other predictor variables are present, bike rentals can still increase by 0.07 units

## Technologies Used

- Python

## Contact

Created by [@prathyu13] - feel free to contact me!
