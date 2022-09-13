# Bike Sharing Assignment
> This is a programming assignment to build a multiple linear regression model for the prediction of demand for shared bikes


## Table of Contents
* [General Info](#general-information)
* [Technologies Used](#technologies-used)
* [Conclusions](#conclusions)
* [Acknowledgements](#acknowledgements)


## General Information

A bike-sharing system is a service in which bikes are made available for shared use to individuals on a short term basis for a price or free. 

A US bike-sharing provider BoomBikes has recently suffered considerable dips in their revenues due to the ongoing Corona pandemic. The company is finding it very difficult to sustain in the current market scenario. So, it has decided to come up with a plan to be able to accelerate its revenue as soon as the ongoing lockdown comes to an end, and the economy restores to a healthy state.

The aim is to understand the factors affecting the demand for these shared bikes in the American market. The company wants to know:

- Which variables are significant in predicting the demand for shared bikes.
- How well those variables describe the bike demands

Following data set have been used for the project

=========================================
Dataset characteristics
=========================================	
day.csv have the following fields:
	
	- instant: record index
	- dteday : date
	- season : season (1:spring, 2:summer, 3:fall, 4:winter)
	- yr : year (0: 2018, 1:2019)
	- mnth : month ( 1 to 12)
	- holiday : weather day is a holiday or not
	- weekday : day of the week
	- workingday : if day is neither weekend nor holiday is 1, otherwise is 0.
	+ weathersit : 
		- 1: Clear, Few clouds, Partly cloudy, Partly cloudy
		- 2: Mist + Cloudy, Mist + Broken clouds, Mist + Few clouds, Mist
		- 3: Light Snow, Light Rain + Thunderstorm + Scattered clouds, Light Rain + Scattered clouds
		- 4: Heavy Rain + Ice Pallets + Thunderstorm + Mist, Snow + Fog
	- temp : temperature in Celsius
	- atemp: feeling temperature in Celsius
	- hum: humidity
	- windspeed: wind speed
	- casual: count of casual users
	- registered: count of registered users
	- cnt: count of total rental bikes including both casual and registered

## Conclusions

The equation of our model fitted line is

cnt = 0.0271 * weekday  -  0.0963 * workingday  +  0.149 * temp  -  0.0470 * hum  -  0.0222 * windspeed  +  0.9394 * registered

Thus we can conlude that:

Count of Bike Rental:

- Increases with increase of Registered users
- Increases when there is Weekdays
- Increases with Temprature
- Decreases with high humidity
- Decreases with high windspeed
- Decreases when Workingday is an non-working day or no working day


## Technologies Used

- pandas
- numpy
- matplotlib
- seaborn
- statsmodels
- sklearn

## Acknowledgements
Give credit here.
- This project is based on Linear Regression Bike Sharing Assignment of UpGrad

## Contact
Created by [@shahebazmadani@gmail.com] - feel free to contact me!
