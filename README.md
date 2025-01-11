Name: K SANJAY

Company: CODTECH IT SOLUTIONS

ID: CT6WECF

Domain: Python programming

Duration: Dec 17 2024 to Jan 17 2025

Mentor: N.SANTHOSH

**Overview of the code:**

**Key Steps**

**API Setup:**

The script interacts with the OpenWeatherMap API, which provides weather data for any location.
You need an API key (a unique identifier) to access the API.

**API Request:**

The script constructs an HTTP GET request to the OpenWeatherMap API using the base URL and query parameters:
City name (q).
API key (appid).
Units (metric for Celsius).

**Fetch Data:**

The requests library sends the GET request and handles the API response.
If the request is successful (status_code 200), the response is parsed as JSON.
If there’s an error (e.g., incorrect city name or invalid API key), an exception is raised and handled gracefully.

**Parse and Display Data:**

Extracts key details from the JSON response:
City name.
Temperature.
Weather description (e.g., "clear sky").
Displays the data in a simple, readable format.

**Key Libraries**

requests:

Handles the HTTP GET request to the API.
Manages exceptions for network or server-related issues.

JSON Handling:

The API response is in JSON format. The script extracts specific fields (e.g., temperature) using dictionary keys.
Outputs

The script prints:

The name of the city.
The current temperature (in Celsius).
A brief description of the weather (e.g., "light rain").

**Example Output**

For CITY = "London":


City: London
Temperature: 15°C
Weather: clear sky

**Key Features**

Modularity:

The code is organized into functions:
fetch_weather: Fetches and parses data.
display_weather: Formats and displays the fetched data.
This modularity makes the code reusable and maintainable.

Error Handling:

Handles potential issues, such as:
Network errors.
Invalid API keys or city names.
Ensures the program doesn’t crash but instead prints an error message.
Customizable:

Easily adaptable for other endpoints or APIs by modifying the base_url and query parameters.

**Use Cases**

Fetch real-time weather data for applications (e.g., weather dashboards or notification systems).
Learn how to interact with REST APIs and handle JSON data.
Adapt the script for other APIs (e.g., news, finance, or sports data).

![Screenshot (81)](https://github.com/user-attachments/assets/93132970-8f0b-40ea-bf01-f340a7f3d81a)
