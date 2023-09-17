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
>  ![image](https://github.com/Bhavya418/Introduction_to_DataMining_CP1_Grp25/assets/85784299/cd587521-cda6-4766-9cfd-00e3de4d7b7e)
> ![image](https://github.com/Bhavya418/Introduction_to_DataMining_CP1_Grp25/assets/85784299/aea6e514-a46b-4993-ae08-d4bc6d92e1ad)


## Exploratory Data Analysis
> First of all, we plotted violin plots to understand the distribution of the features.
> Then we plotted different plots to understand the relationship between different features such as linear relationship which features are more important than others.
> - The plots for the following can be found in the file.
> - Certain important plots:
>  ![image](https://github.com/Bhavya418/Introduction_to_DataMining_CP1_Grp25/assets/85784299/a643d71b-88a0-4fbb-a21c-b4688c8687e3)

>  ![image](https://github.com/Bhavya418/Introduction_to_DataMining_CP1_Grp25/assets/85784299/d5c8e1aa-c09b-456e-adae-d6e7edf57b16)

>  ![image](https://github.com/Bhavya418/Introduction_to_DataMining_CP1_Grp25/assets/85784299/c891bf68-34e4-4cbb-b593-0c5715aa6d73)

>  ![image](https://github.com/Bhavya418/Introduction_to_DataMining_CP1_Grp25/assets/85784299/6fea5837-4479-4875-9c62-b7ede8f6826a)
  
## Machine Learning and Data Transformations

> - We performed two data transformation techniques :
>   1. Standardization using z-score
>   2. Normalization using min-max score
>      
> Then as the 





