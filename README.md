# Unit 6 Homework: What's the Weather Like?

## Background

Whether financial, political, or social&mdash;data's true power rests in its ability to answer questions definitively. This module challenge is a display of my understanding of the concepts of Python requests, APIs, and JSON traversals to answer a fundamental question: "What's the weather like as we approach the equator?"

Now, we know what you may be thinking: _"Duh. It gets hotter ..."_

But, if pressed, how would you **prove** it?


## Part 1: WeatherPy

In this section, a Python script was created to visualize the weather of 500+ cities of varying distance from the equator. A [simple Python library](https://pypi.python.org/pypi/citipy), the [OpenWeatherMap API](https://openweathermap.org/api), was used to create a representative model of weather across cities.

The following scatter plots were generated to showcase the following relationships:

* Temperature (F) vs. Latitude
* Humidity (%) vs. Latitude
* Cloudiness (%) vs. Latitude
* Wind Speed (mph) vs. Latitude

The linear regression for each relationship is computed. the plots are separated into Northern Hemisphere (greater than or equal to 0 degrees latitude) and Southern Hemisphere (less than 0 degrees latitude):

* Northern Hemisphere - Temperature (F) vs. Latitude
* Southern Hemisphere - Temperature (F) vs. Latitude
* Northern Hemisphere - Humidity (%) vs. Latitude
* Southern Hemisphere - Humidity (%) vs. Latitude
* Northern Hemisphere - Cloudiness (%) vs. Latitude
* Southern Hemisphere - Cloudiness (%) vs. Latitude
* Northern Hemisphere - Wind Speed (mph) vs. Latitude
* Southern Hemisphere - Wind Speed (mph) vs. Latitude


### Part 2: VacationPy

Jupyter-gmaps and the Google Places API was used to plan future vacations. 


* A heat map was created that displays the humidity for every city from Part 1, as in the following image:

  ![heatmap](Images/heatmap.png)

* The DataFrame was narrowed down to find your ideal weather condition. For example:

  * A max temperature lower than 80 degrees but higher than 70.

  * Wind speed less than 10 mph.

  * Zero cloudiness.

  * Rows that didn't  satisfy all three conditions were dropped to ensure the weather is ideal.

* Google Places API was used to find the first hotel for each city located within 5,000 meters of the coordinates.

* The hotels on top of the humidity heatmap, with each pin containing the **Hotel Name**, **City**, and **Country**, as in the following image, were plotted:

  ![hotel map](Images/hotel_map.png)

- - -

© 2022 Trilogy Education Services, a 2U, Inc. brand. All Rights Reserved.