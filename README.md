# python-api-challenge

## Part I - WeatherPy

In this example, you'll be creating a Python script to visualize the weather of 500+ cities across the world of varying distance from the equator. To accomplish this, you'll be utilizing a [simple Python library](https://pypi.python.org/pypi/citipy), the [OpenWeatherMap API](https://openweathermap.org/api), and a little common sense to create a representative model of weather across world cities.

The first requirement is to create a series of scatter plots to showcase the following relationships:

* Temperature (F) vs. Latitude

<p align="center">
  <img src="/Images/temperature%20vs%20latitude%20(all).png" />
</p>
 
We can see there is a clear correlation between temperature and latitude. As we approach the equator (latitude values near zero), the temperature increases. On the other side, as we approach the poles (latitude values near -90 or near 90), temperature decreases.
 
 
* Humidity (%) vs. Latitude

<p align="center">
  <img src="/Images/humidity%20vs%20latitude%20(all).png" />
</p>

In this case, no clear correlation can be seen between humidity and latitude.


* Cloudiness (%) vs. Latitude

<p align="center">
  <img src="/Images/cloudiness%20vs%20latitude%20(all).png" />
</p>

In this case, no clear correlation can be seen between cloudiness and latitude.


* Wind Speed (mph) vs. Latitude

<p align="center">
  <img src="/Images/wind%20speed%20vs%20latitude%20(all).png" />
</p>

<br><br>

In this case, no clear correlation can be seen between wind speed and latitude.

The second requirement is to run linear regression on each relationship. This time, separate the plots into Northern Hemisphere (greater than or equal to 0 degrees latitude) and Southern Hemisphere (less than 0 degrees latitude):

* Northern Hemisphere - Temperature (F) vs. Latitude
<p align="center">
  <img src="/Images/temperature%20vs%20latitude%20(north).png" />
</p>

* Southern Hemisphere - Temperature (F) vs. Latitude
<p align="center">
  <img src="/Images/temperature%20vs%20latitude%20(south).png" />
</p>

* Northern Hemisphere - Humidity (%) vs. Latitude
<p align="center">
  <img src="/Images/humidity%20vs%20latitude%20(north).png" />
</p>

* Southern Hemisphere - Humidity (%) vs. Latitude
<p align="center">
  <img src="/Images/humidity%20vs%20latitude%20(south).png" />
</p>

* Northern Hemisphere - Cloudiness (%) vs. Latitude
<p align="center">
  <img src="/Images/cloudiness%20vs%20latitude%20(north).png" />
</p>

* Southern Hemisphere - Cloudiness (%) vs. Latitude
<p align="center">
  <img src="/Images/cloudiness%20vs%20latitude%20(south).png" />
</p>

* Northern Hemisphere - Wind Speed (mph) vs. Latitude
<p align="center">
  <img src="/Images/wind%20speed%20vs%20latitude%20(north).png" />
</p>

* Southern Hemisphere - Wind Speed (mph) vs. Latitude
<p align="center">
  <img src="/Images/wind%20speed%20vs%20latitude%20(south).png" />
</p>

<br><br>

### Part II - VacationPy

Now let's use your skills in working with weather data to plan future vacations. Use jupyter-gmaps and the Google Places API for this part of the assignment.

* **Note:** Remember that any API usage beyond the $200 credit will be charged to your personal account. You can set quotas and limits to your daily requests to be sure you can't be charged. Check out [Google Maps Platform Billing](https://developers.google.com/maps/billing/gmp-billing#monitor-and-restrict-consumption) and [Manage your cost of use](https://developers.google.com/maps/documentation/javascript/usage-and-billing#set-caps) for more information.

* **Note:** if you having trouble displaying the maps, try running `jupyter nbextension enable --py gmaps` in your environment and retry.

To complete this part of the assignment,you will need to do the following:

* Create a heat map that displays the humidity for every city from Part I.

<p align="center">
  <img src="/Images/heatmap_humidity.png" />
</p>

* Narrow down the DataFrame to find your ideal weather condition and using Google Places API to find the first hotel for each city located within 5000 meters of your coordinates. Plot the hotels on top of the humidity heatmap with each pin containing the **Hotel Name**, **City**, and **Country**.

<p align="center">
  <img src="/Images/map_hotels.png" />
</p>
