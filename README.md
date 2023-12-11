``` | Bek Brace Channel Video Tutorial | Video Tutorial for November 2023 ```

# weather_app_pyramid_fw

🌦️ **Weather Application Powered by Pyramid Framework for Python** 🐍🔼

Experience the magic of the Pyramid Framework for Python with our Weather App! This web application empowers users to check real-time weather conditions for any city, providing essential data such as temperature, weather description (e.g., sunny, cloudy, rainy), humidity, pressure, and wind speed. Users can simply input a city name, and the app seamlessly fetches and displays the weather information, leveraging data from OpenWeatherMap.

Key features of the Weather App:

Real-Time Data: The app fetches up-to-date weather data for the specified city, ensuring precision and currency.

User-Friendly: Crafted with user-friendliness in mind, the interface boasts an intuitive form for effortlessly entering the city name.

Weather Icons(in process): Visual icons make it a breeze for users to grasp weather conditions at a glance, all thanks to the Pyramid Framework's flexibility.

Customization: Personalize your experience! Users can easily customize the city they want to check the weather for.

The Weather App is your go-to tool for swiftly checking the weather conditions for a specific location, be it for travel planning, daily routines, or simply staying informed about the ever-changing weather.

Technologies Used:

Python
Pyramid (for the web application)
Jinja2 (for rendering HTML templates)
OpenWeatherMap API (for weather data)


```Installation```
Clone this repository to your local machine:

```bash
git clone https://github.com/BekBrace/weather_app_pyramid_fw/tree/main
```

Navigate to the project directory:
```console
cd weather_app_pyramid_fw
```
Create a virtual environment and activate it (recommended):
pipenv shell

Install the required dependencies using pipenv:
```console
pipenv install requests pyramid cookiecutter
```

```Cookiecutter is a popular tool for creating project templates in Python. It allows you to create project skeletons from predefined templates quickly. If you want to create a Pyramid web application using Cookiecutter, you can use a Cookiecutter template specifically designed for Pyramid applications. One such template is the "cookiecutter-pyramid" template.```

Configure your OpenWeatherMap API key:

Create a profile, get your API key from https://openweathermap.org

Open the weatherapp/views.py file and replace 'YOUR_API_KEY' with your actual OpenWeatherMap API key.

Make your application available for Dev and Testing:
```console
python setup.py develop
```
Start the Pyramid application:
```console
pserve development.ini --reload
```
Usage
After installing and starting the application, you can access it by opening a web browser and navigating to http://localhost:6543/. You will see a simple web page that allows you to enter a city name and retrieve its weather information.

How it Works
This Pyramid application consists of two views defined in the weatherapp/views.py file:

home: This view renders the home page, where users can enter a city name.

weather: This view handles the weather information retrieval. It sends a request to the OpenWeatherMap API with the specified city name, and then it parses the JSON response to extract relevant weather data such as temperature, description, humidity, pressure, and wind speed. The weather data is then passed to the template for rendering.

Dependencies
This application relies on the following Python libraries and frameworks:

Pyramid: A Python web framework.
Requests: A Python library for making HTTP requests.
Configuration
The configuration for the Pyramid application is stored in the development.ini file. You can customize the settings such as the server port, host, and database connection if needed.

Credits
This application was created by [Your Name].
License
This project is licensed under the MIT License. See the LICENSE file for details.
