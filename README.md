# PYTHON API's
## Purpose
I created a Python script to visualize the weather of 500+ cities across the world of varying distance from the equator. To accomplish this, I utilized a simple Python library, the OpenWeatherMap API, and a little common sense to create a representative model of weather across world cities.

## Process
1. First I created a series of scatter plots to showcase the following relationships:

 * Temperature (F) vs. Latitude
 * Humidity (%) vs. Latitude
 * Cloudiness (%) vs. Latitude
 * Wind Speed (mph) vs. Latitude

2. Then I ran a linear regression on each relationship and seperated the plots into Northern Hemisphere (greater than or equal to 0 degrees latitude) and Southern Hemisphere (less than 0 degrees latitude):

 * Northern Hemisphere - Temperature (F) vs. Latitude
 * Southern Hemisphere - Temperature (F) vs. Latitude
 * Northern Hemisphere - Humidity (%) vs. Latitude
 * Southern Hemisphere - Humidity (%) vs. Latitude
 * Northern Hemisphere - Cloudiness (%) vs. Latitude
 * Southern Hemisphere - Cloudiness (%) vs. Latitude
 * Northern Hemisphere - Wind Speed (mph) vs. Latitude
 * Southern Hemisphere - Wind Speed (mph) vs. Latitude

3. I randomly selected at least 500 unique (non-repeat) cities based on latitude and longitude,
Performed a weather check on each of the cities using a series of successive API calls,
Included a print log of each city as it's being processed with the city number and city name, and
Saved a CSV of all retrieved data and a PNG image for each scatter plot.
