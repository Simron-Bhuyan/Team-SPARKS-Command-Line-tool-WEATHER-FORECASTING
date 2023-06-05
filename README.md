# Command-Line-tool--WEATHER-FORECASTING

This tool allows you to fetch weather and temperature information for multiple cities by using the OpenWeather API to retrieve the data.

**Code Overview**

The code is written in Python and utilizes several modules and libraries.
It follows a modular approach with well-defined functions.
Let's go through the key components and functionalities of the code.

**Command-Line Interaction**

The code interacts with the user through the command-line interface (CLI).
It uses the argparse module to handle user input.
Users can specify the number of cities to check and choose to display the temperature in imperial units.

**Building the Weather Query URL**

The code constructs the API request URL for each city using the build_weather_query() function.
It takes the city name and a flag for imperial units as input.
The API key is fetched from a configuration file named "secrets.ini".
The URL is formatted with the city name, units, and API key.

**Making API Requests**

The get_weather_data() function makes an API request to the OpenWeather API using the constructed URL.
It handles potential HTTP errors, such as unauthorized access or city not found.
The response data is returned as a Python dictionary.
