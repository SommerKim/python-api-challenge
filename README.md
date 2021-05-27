# Weather Analysis

This project seeks to find an ideal vacation spot based on weather patterns and preferences by filtering API call results based on certain weather criteria and plotting the results to a map.

In WeatherPy, I examined weather behaviors from different parts of the world. I pulled data from the OpenWeatherMap API to look for correlation between one of four weather features (temperature, humidity, cloudiness and wind speed) and latitudinal location. Using randomly selected cities to guide my API search, I gathered each city's country, date, latitude, longitude, temperature, humidity level, cloudiness, and current wind speeds for a dataframe, then exported the data to a .csv file. 

The scatter plots created from the dataframe revealed a noticeable trend for temperature of a location according to its latitude-- namely, that temperature is generally higher in cities that are closer to the equator. Calculating the r-value confirmed the correlation.

In the second part of the challenge, VacationPy, I built on the information found in WeatherPy to find an ideal place to vacation based on weather. Using the .csv file created for WeatherPy, I created a heatmap of my random city locations by using jupyter-gmaps. From there, I narrowed down the potential vacation spots by filtering the dataframe according to my preferences for temperature, cloudiness and wind speed. Using this new, smaller set of data, I used the Google Places API to find a hotel in each ideal location. Then, I created a marker layer for my map depicting the locations of the hotels.

<img width="726" alt="heatmap_w_markers" src="https://user-images.githubusercontent.com/74261427/119834198-bd64b900-becd-11eb-8b2b-a88a9d2f3d35.PNG">
<img width="331" alt="city_lat_vs_max_temp" src="https://user-images.githubusercontent.com/74261427/119834241-c6ee2100-becd-11eb-849b-c0bdf769da88.PNG">
<img width="321" alt="north_lat_temp_regression" src="https://user-images.githubusercontent.com/74261427/119834259-cb1a3e80-becd-11eb-89dc-0eba7ec5cd20.PNG">
