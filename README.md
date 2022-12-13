# World_Weather_Analysis
Module6

## Overview
This analysis consists of three parts, creating a database showing 2000 random cities to map by max temperature, building a searchable database that filters on desired temperature, and mapping out an itinerary for traveling to four cities.

### The Weather Database
This database consists of about 2000 cities randomly generated. A connection to openweathermap.org was created to pull live data on:
- Latitude and Longitude
- Maximum Temperature
- Humidity
- Cloudiness
- Wind Speed
- Current Description

### Travel Destinations Map
The above data points were built into a DataFrame to provide a database where users could choose travel destinations based on temperature. Filters were built into the python code to allow a user to input their desired min and max temperatures, and the code returned any city with a max temp within that range. Once the range was decided, a GeoViews map was created to visualize the results. 

![WeatherPy_vacation_map](https://user-images.githubusercontent.com/114450503/207230809-af14b702-18c0-40da-8523-71d2b0f17c8d.png)

### Itinerary Map
Now that the GeoView map showed travel destinations with the desired temperature, the user could zoom in on various areas of the world to finally decide the details of their trip. Settling on four cities reasonably close to each other, a route was established using the Geoapify Routing API. The coordinates were gathered and mapped to provide a custom map of the four cities the user wished to visit. 

![WeatherPy_travel_map](https://user-images.githubusercontent.com/114450503/207231363-b82a9f51-6b1d-42cf-bd47-afceddca231a.png)

### Conclusion
One of the benefits of using an API as shown above is it's ability to pull real-time data. Instead of having static data that would only be accurate for a month at a time, this code could be used without modification year-round and still provide users accurate data. 

Another benefit of APIs is it's ability to incorporate "other" data that a developer may not locally have access to, and the opportunities that presents to enrich a dataset and provide more information to its users. This exercise could have started with a travel-center and their customers' recorded trips for the last year and then introduced a new database that the sales reps could tap into to market new exciting travel locations. 
