# PYTHON API CHALLENGE:

## OBSERVATIONS & TRENDS:

After analyzing the weather of 559 randomly selected global cities, the following observations and trends were made as Of March 14, 2020.  Most of the cities (382 out of the total 547) were randomly selected in the Northern Hemisphere or 68% of the total cities and the remaining 177 cities were in the Southern Hemisphere.

1) As one might expect, the higher the latitude above the equator, then the lower the temperatures (F) would be across the cities and vice versa.  This is proven by the high correlation of -0.91 between latitude and temperature in the Northern Hemisphere and the moderate correlation of 0.63 in the Southern Hemisphere. The strongest correlated values are -1 and +1 and the weakest correlation is zero with no relationship between two variables.  Since the Northern Hemisphere has a very strong negative correlation of -0.91, this indicates that as the latitude reaches higher towards the North Pole (for example), then the temperatures will become lower and as the latitude moves closer to the equator, then the temperatures rise.

2) There is a weak correlation between latitude and humidity values in both the Northern and Southern Hemispheres with values of 0.21 and 0.23, respectively.  Humidity is much higher as one approaches the equator.

3) There is a very weak correlation between latitude and cloudiness values in both the Northern and Southern Hemispheres with values of 0.13 and 0.21, respectively.  However, it is interesting to note that you see straight line clusters of cloudiness around 0%, 40% and in between 80% to 100%.

4) There is a fairly weak correlation between latitude and wind speed in both the Northern and Southern Hemispheres with values of 0.23 and -0.30, respectively.  Wind speeds tend to cluster around 0-15 mph irrespective of latitude.




## BACKGROUND


## Part I - WeatherPy

Created a Python script to visualize the weather of 500+ cities across the world of varying distance from the equator. 

The first objective was to build a series of scatter plots to showcase the following relationships:

* Temperature (F) vs. Latitude
* Humidity (%) vs. Latitude
* Cloudiness (%) vs. Latitude
* Wind Speed (mph) vs. Latitude

The next objective was to run linear regression on each relationship, only this time separating them into Northern Hemisphere (greater than or equal to 0 degrees latitude) and Southern Hemisphere (less than 0 degrees latitude):

* Northern Hemisphere - Temperature (F) vs. Latitude
* Southern Hemisphere - Temperature (F) vs. Latitude
* Northern Hemisphere - Humidity (%) vs. Latitude
* Southern Hemisphere - Humidity (%) vs. Latitude
* Northern Hemisphere - Cloudiness (%) vs. Latitude
* Southern Hemisphere - Cloudiness (%) vs. Latitude
* Northern Hemisphere - Wind Speed (mph) vs. Latitude
* Southern Hemisphere - Wind Speed (mph) vs. Latitude

### Part II - VacationPy

* Created a heat map that displays the humidity for every city from the part I.

  ![heatmap](Images/heatmap.png)

* Narrowed down the DataFrame to find the ideal weather condition. For example:

  * A max temperature lower than 80 degrees but higher than 70.

  * Wind speed less than 10 mph.

  * Zero cloudiness.

  * Dropped any rows that didn't contain all three conditions to be sure the weather was ideal.