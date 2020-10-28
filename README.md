# Python-API
## What's the Weather Like?

Let's take what we know about Python requests, APIs, and JSON traversals to answer a fundamental question: "What's the weather like as we approach the equator?"

## Part I - WeatherPy
In this example, I'll be creating a Python script to visualize the weather of 500+ cities across the world of varying distance from the equator. To accomplish this, I'll be utilizing a simple Python library, the OpenWeatherMap API, and a little common sense to create a representative model of weather across world cities.

1. Create a series of scatter plots to showcase the following relationships:
</br>- Temperature (F) vs. Latitude
</br>- Humidity (%) vs. Latitude
</br>- Cloudiness (%) vs. Latitude
</br>- Wind Speed (mph) vs. Latitude

2. Run linear regression on each relationship, only this time separating them into Northern Hemisphere (greater than or equal to 0 degrees latitude) and Southern Hemisphere (less than 0 degrees latitude):
</br>- Northern Hemisphere - Temperature (F) vs. Latitude
</br>- Southern Hemisphere - Temperature (F) vs. Latitude
</br>- Northern Hemisphere - Humidity (%) vs. Latitude
</br>- Southern Hemisphere - Humidity (%) vs. Latitude
</br>- Northern Hemisphere - Cloudiness (%) vs. Latitude
</br>- Southern Hemisphere - Cloudiness (%) vs. Latitude
</br>- Northern Hemisphere - Wind Speed (mph) vs. Latitude
</br>- Southern Hemisphere - Wind Speed (mph) vs. Latitude

The final notebook must:
</br>- Randomly select at least 500 unique (non-repeat) cities based on latitude and longitude.
</br>- Perform a weather check on each of the cities using a series of successive API calls.
</br>- Include a print log of each city as it's being processed with the city number and city name.
</br>- Save a CSV of all retrieved data and a PNG image for each scatter plot.

## Part II - VacationPy
Now let's plan future vacations. I will use jupyter-gmaps and the Google Places API for this part.

Note: if you having trouble displaying the maps try running jupyter nbextension enable --py gmaps in your environment and retry.

1. Create a heat map that displays the humidity for every city from the part I.

2. Narrow down the DataFrame to find the ideal weather condition. For example:
</br>- A max temperature lower than 80 degrees but higher than 70.
</br>- Wind speed less than 10 mph.
</br>- Zero cloudiness.
</br>- Drop any rows that don't contain all three conditions. You want to be sure the weather is ideal.

Note: Adjusting specifications is allowed, but I'll be sure to limit the number of rows returned by my API requests to a reasonable number.

3. Using Google Places API to find the first hotel for each city located within 5000 meters of my coordinates.

4. Plot the hotels on top of the humidity heatmap with each pin containing the Hotel Name, City, and Country.


