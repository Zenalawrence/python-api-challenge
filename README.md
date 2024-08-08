# python-api-challenge

## WeatherPy

Python requests, APIs, and JSON traversals were used to answer the weather question: "What's the weather like as we approach the equator?"

### Summary
A sample set of 500 cities were randomly selected from a list using citipy python library.

**Latitude vs. Temperature:**

The northern hemisphere displays a negative correlation as latitude increases from 0 to 50 degrees, the temperature decreases.  The southern hemisphere shows a positive correlation as latitude increases from -50 to 0 degress, temperature increases.  This is known to be true as we more closer to the equator at 0deg, the temperatures are warmer.  The R<sup>2</sup> values are 0.45 and 0.61 respectively which indicates that this is relatively true for most of our data since they are close to each other.

**Latitude vs. Humidity:**

There is no direct correlation between humidity and latitude.  Both the northern and southern hemisphere has similar humidity as we increase in latitude(or move closer to the equator).  They have a R<sup>2</sup> value of 0.0004 and 0.01 respectively which are both quite small.  This indicated the data is spread out, further strengthening the finding that humidity is not affected by latitude. The norhern hemisphere has appears to be more dense, but this may be to us randomly selecting more cities in the northern hemisphere. 

**Latitude vs. Cloudiness:**

The data is right skewed as we move closer to the equator(0deg latitude), we see more clouds for the southern hemisphere.  This may be because the data was taken in August, the southern hemisphere maybe experiencing winter at -50deg latitude, and rainy season at 0deg latitude.  The Northern hemisphere appears to not have a direct correlation between cloudiness and latitude.  They have a R<sup>2</sup> value of 0.021 and 0.0082 respectively which are both quite small.  This proves there is not a strong correlation between cloudiness and latitude.

**Latitude vs. Wind Speed:**

Wind speeds are mostly below 6 m/s in the northern hemisphere as we move closer to the equator.  This differs in the southern hemisphere as wind speed range from 0 to 12 m/s.  There is not a direct correlation between wind speeds and latitude.


## VacationPy

GeoViews Python library and Geoapigy API was used to generate a list of Hotels in my list of different countries that meet my specific weather requirements.  These requirements were based on the weather conditions in these countries.


## References for code used in this challenge:

**Weather API**
https://openweathermap.org/current#name

**matplotlib scatter plot guide**
https://matplotlib.org/stable/api/_as_gen/matplotlib.pyplot.scatter.html

**axis grid document**
https://matplotlib.org/stable/api/_as_gen/matplotlib.axes.Axes.grid.html

**linregress document**
https://docs.scipy.org/doc/scipy/reference/generated/scipy.stats.linregress.html