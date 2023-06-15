###              Module 6 : Python API -- WEATHERPY

## Introduction:
Data's true power is its ability to definitively answer questions. So, let's see how Python requests, APIs, and JSON traversals to answer a fundamental question: "What is the weather like as we approach the equator?"
Now, we know what you may be thinking: “That’s obvious. It gets hotter.” But, if pressed for more information, how would you prove that?

## Instructions: 
This activity is broken down into two deliverables, WeatherPy and VacationPy.

# Part 1: WeatherPy
Create a Python script to visualize the weather of over 500 cities of varying distances from the equator. You'll use the citipy Python libraryLinks to an external site., the OpenWeatherMap APILinks to an external site., and your problem-solving skills to create a representative model of weather across cities.

# Requirement 1: Create Plots to Showcase the Relationship Between Weather Variables and Latitude
To fulfill the first requirement, use the OpenWeatherMap API to retrieve weather data from the cities list generated in the starter code. Next, Create a series of scatter plots to showcase the following relationships:
Latitude vs. Temperature
Latitude vs. Humidity
Latitude vs. Cloudiness
Latitude vs. Wind Speed

# Requirement 2: Compute Linear Regression for Each Relationship
Compute the linear regression for each relationship. Separate the plots into Northern Hemisphere (greater than or equal to 0 degrees latitude) and Southern Hemisphere (less than 0 degrees latitude). You may find it helpful to define a function in order to create the linear regression plots.
Next, create a series of scatter plots. Be sure to include the linear regression line, the model's formula, and the r values 
Sample scatter plot with the linear regression line.

Northern Hemisphere: Temperature vs. Latitude
Southern Hemisphere: Temperature vs. Latitude
    Northern Hemisphere: Humidity vs. Latitude
    Southern Hemisphere: Humidity vs. Latitude
        Northern Hemisphere: Cloudiness vs. Latitude
        Southern Hemisphere: Cloudiness vs. Latitude
            Northern Hemisphere: Wind Speed vs. Latitude
            Southern Hemisphere: Wind Speed vs. Latitude

## Part 2: VacationPy
Use your weather data skills to plan future vacations. Also, you'll use Jupyter notebooks, the geoViews Python library, and the Geoapify API.
The code needed to import the required libraries and load the CSV file with the weather and coordinates data for each city created in Part 1 is provided to help you get started.
Your main tasks will be to use the Geoapify API and the geoViews Python library and employ your Python skills to create map visualizations.
To succeed on this deliverable of the assignment, open the VacationPy.ipynb starter code and complete the following steps:

# Create a map that displays a point for every city in the city_data_df DataFrame as shown in the following image. The size of the point should be the humidity in each city.
Humidity map
    A max temperature lower than 27 degrees but higher than 21
    Wind speed less than 4.5 m/s
    Zero cloudiness

## Create a new DataFrame called hotel_df to store the city, country, coordinates, and humidity.
For each city, use the Geoapify API to find the first hotel located within 10,000 meters of your coordinates.
Add the hotel name and the country as additional information in the hover message for each city on the map as in the following image:

Hotel map
Hints and Considerations
The city data that you generate is based on random coordinates and different query times, so your outputs will not be an exact match to the provided starter notebook.


# Hint: Consider the full range of latitudes.
Once you have computed the linear regression for one relationship, you will follow a similar process for all other charts. Optionally, try to create a function that will create these charts based on different parameters. (Note: there will be no extra points for completing this.)

Remember that each coordinate will trigger a separate call to the Google API. If you're creating your own criteria to plan your vacation, try to reduce the results in your DataFrame to 10 or fewer cities.

© 2022 edX Boot Camps LLC. Confidential and Proprietary. All Rights Reserved.
