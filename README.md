# Introduction_to_DataMining_CP1_Grp25

# **Seoul Bike Trip**
> The most basic metric for all forms of transportation is trip length. Therefore, accurate trip-time prediction is essential for the development of Intelligent Transportation Systems (ITS) and traveller information systems. In order to forecast the duration of a journey, we used certain optimized data mining techniques to forecast the duration of trips involving rental bikes in the bike-sharing programme in Seoul. The forecast is made using a combination of weather data and Pickup and Drop location data.


## Introduction

> There are 1284153 data instances and 26 features.
> The Data used include trip duration, trip distance, pickup-dropoff latitude and longitude, temperature, precipitation, wind speed, humidity, solar radiation, snowfall, ground temperature and 1-hour average dust concentration.
> 1. **Trip Duration**: It represents the duration of a bike trip in some unit of time, such as minutes or seconds.
> 1. **Trip Distance**: The distance covered during the bike trip, typically measured in kilometres or miles. This feature can help in understanding how to trip duration relates to the distance traveled.
> 1. **Pickup and Dropoff Latitude and Longitude**: These are geographical coordinates representing the exact location where the bike trip starts (pickup) and ends (dropoff). Latitude and longitude are used to pinpoint specific locations on the Earth's surface.
> 1. **Temperature**: The temperature at the time of the trip, usually measured in degrees Celsius or Fahrenheit. It can provide insights into how weather conditions affect trip duration.
> 1. **Precipitation**: This feature indicates whether there was any form of precipitation (rain, snow, etc.) during the trip. It's often represented as a binary variable (0 for no precipitation, 1 for precipitation).
> 1. **Wind Speed**: The speed of the wind at the time of the trip, measured in units like kilometres per hour (km/h) or meters per second (m/s). Wind speed can influence the ease of cycling.
> 1. **Humidity**: The level of moisture or humidity in the air during the trip, often represented as a percentage. High humidity can affect comfort during cycling.
> 1. **Solar Radiation**: Solar radiation measures the amount of energy received from the sun during the trip. It's typically measured in watts per square meter (W/m²) and can impact temperature and weather conditions.
> 1. **Snowfall**: Indicates whether there was snowfall during the trip, usually represented as a binary variable (0 for no snowfall, 1 for snowfall). Snowfall can significantly affect road conditions and trip duration.
> 1. **Ground Temperature**: The temperature of the ground or road surface at the time of the trip. This can be important, especially in cold or icy conditions.
> 1. **1-Hour Average Dust Concentration**: This feature represents the concentration of particulate matter (dust) in the air, typically measured in micrograms per cubic meter (µg/m³). It provides information about air quality, which can affect health and comfort during the trip.

## Data Preprocessing 
> - The first step is to check a number of null values and either replace them or remove them.
> - The second step is to remove the outliers from the dataset which are important and possibly have unwanted instances.
> - The third step is to remove the correlated features by plotting the heatmap and removing the features with a correlation greater than 80%.
>   
>  ![image](https://github.com/Bhavya418/Introduction_to_DataMining_CP1_Grp25/assets/85784299/36809aac-99d4-4141-8e2c-0b70c0a90bb7)

> ![image](https://github.com/Bhavya418/Introduction_to_DataMining_CP1_Grp25/assets/85784299/5f421047-9ee2-461b-9b44-8359c7bcc326)



## Exploratory Data Analysis
> First of all, we plotted violin plots to understand the distribution of the features.
> Then we plotted different plots to understand the relationship between different features such as linear relationships which features are more important than others.
> - The plots for the following can be found in the file.
> - Certain important plots:

>  ![image](https://github.com/Bhavya418/Introduction_to_DataMining_CP1_Grp25/assets/85784299/5330fd05-90dd-4e0a-8f83-07401872df7c)
  
>  ![image](https://github.com/Bhavya418/Introduction_to_DataMining_CP1_Grp25/assets/85784299/0b1ea625-affc-483b-b367-739075a63e0e)

>  ![image](https://github.com/Bhavya418/Introduction_to_DataMining_CP1_Grp25/assets/85784299/f1b801dd-32bd-4a7f-bda9-e5bfcfc8bd4c)

>  ![image](https://github.com/Bhavya418/Introduction_to_DataMining_CP1_Grp25/assets/85784299/ce62e1f7-f671-475e-b467-b2e9a029db03)

> ![image](https://github.com/Bhavya418/Introduction_to_DataMining_CP1_Grp25/assets/85784299/939063f4-f853-472f-ab85-36c8e502e122)

  
## Machine Learning and Data Transformations

> - We performed two data transformation techniques :
>   1. Standardization using z-score
>   2. Normalization using min-max score
>      
> Then as the dataset has been transformed and the unwanted features have been removed, we decided that we would predict the duration of the trip as that would benefit the bike rental about 

> Different Models that we trained
> 1. Linear Regression
> 2. Polynomial Regression
> 3. Random Forest Regressor
> 4. Gradient Boosting Linear Regression
> 5. XGB Booster 

> - We even did some feature engineering and optimization techniques where we tried considering the weather, trained the model and obtained a good RMSE score, absolute error and accuracy.


