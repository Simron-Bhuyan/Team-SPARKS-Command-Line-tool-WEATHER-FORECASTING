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

**Displaying Weather Information**

The display_weather_info() function formats the retrieved weather data.
It extracts relevant information like city name, weather condition ID, description, and temperature.
The weather condition ID is mapped to an appropriate weather symbol and display color.

**Tabulating the Data**

The code utilizes the tabulate function to create a table from the formatted weather data.
Headers for the table include City, Weather, Description, and Temperature.
The table is printed to the console, providing a clear overview of the weather information for each city.

**Demo**

Let's see a demo of the Weather Information Tool in action.
We'll enter a few cities, and the tool will fetch and display the weather information for each city.

**Conclusion**

The Weather Information Tool is a helpful utility for checking weather and temperature information.
It offers command-line interactivity, flexibility with units, and a user-friendly display.
You can explore and customize the code to suit your specific needs.

**Future Scope**
1. Implementing more features like weather conditions like moisture content and more.