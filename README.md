# API-INTEGRATION
*COMPANY*: CODTECH IT SOLUTIONS
*NAME*: SAINATH DIGAMBAR WAKHURE
*INTERN ID*: CT12WSAF
*DOMAIN*:  Full Stack Web Development
*DURATION*: 12 WEEKS 
*MENTOR*: NEELA SANTOSH KUMAR
*API Integration Task of integrating public API of an weather app using public api id*

This project is a  *Weather Application* that allows users to check the current weather and a 5-day forecast for any city they enter. It is built using HTML, CSS, and JavaScript, and uses the WeatherAPI service to fetch live weather data.

- How the API Integration Works
When a user visits the website, they are greeted with a neat and clean layout. There is a navigation bar at the top that says Weather App, and below that, there is a section where the user can input the name of any city. Next to the input field is a button labeled Get Weather.

When the user types in a city name and clicks the button, the JavaScript function called getWeather() gets triggered. This function is responsible for handling the API integration.

First, the function reads the city name entered by the user. It checks if the input is empty — if it is, it shows an alert asking the user to enter a city name.

If a city name is provided, the function prepares two URLs to send requests:

Current Weather URL – This URL fetches the current weather conditions like temperature, wind speed, and the general weather condition (like sunny, rainy, etc.).

Forecast URL – This URL fetches the weather forecast for the next 5 days.

Both URLs include an API key (5611c5f6ef9c432fa8a102633252103) which is required to access the WeatherAPI services.

The fetch() method is then used to send HTTP requests to these URLs.

The first fetch() call gets the current weather data.

When the response is received, it is converted into JSON format.

After that, specific details like the city name, country, temperature (in Celsius), wind speed (in kilometers per hour), and weather condition (with an icon) are extracted.

These details are then dynamically displayed inside the webpage, inside a container with the ID weather.

After displaying the current weather, another fetch() call is made to get the 5-day forecast data.

Again, the response is converted to JSON.

A loop runs through each day in the forecast, and for each day, it shows:

The date

The average temperature

A short description of the weather (like "Partly Cloudy", "Rain", etc.)

An icon representing the weather condition

This forecast information is displayed inside a different container with the ID forecast.

In case there is an error while fetching the data (for example, if the city name is wrong or the API server is down), a friendly error message is shown to the user.

About the Design
The HTML structure is very clean and uses Bootstrap 5 for quick and responsive design. It ensures that the app looks good on both mobile devices and desktops.

The CSS (in styles.css) customizes the look a bit more by:

Setting a nice, light background color.

Centering the weather and forecast information.

Adding some padding, rounded corners, and subtle shadow effects to the weather cards to make them look neat and professional.

The forecast items are displayed in a row, with each day's forecast shown in a small, stylish box.

Summary
In simple words, this weather app takes a city name from the user, sends two requests to WeatherAPI:

one to get current weather

another to get the 5-day forecast

It then shows this information nicely on the webpage. The app handles missing input and errors properly, making it user-friendly. It uses modern tools like fetch() for API requests, and Bootstrap + custom CSS for a good-looking design.

This is a great example of how you can integrate third-party APIs into a basic web application to create something useful and interactive.

#Output: 
![Image](https://github.com/user-attachments/assets/f12d142b-0c38-40ae-bbc4-cb3ed263e842)
