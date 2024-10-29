# Weather API Application

This is a Flask web application that allows users to get current weather information for a specified city, as well as compare the weather between two cities. It retrieves data from the OpenWeatherMap API and displays it in a user-friendly interface.

## Features

- **Current Weather Data:** Users can enter a city name to get current weather conditions, including temperature, humidity, wind speed, sunrise, and sunset times.
- **City Comparison:** Users can compare the weather of two cities side by side.
- **User-Friendly Interface:** Simple forms for input and results displayed in an organized manner.

## Tech Stack

- **Flask:** A lightweight WSGI web application framework in Python.
- **OpenWeatherMap API:** For retrieving weather data.
- **HTML/CSS:** For front-end templates and styling.
- **dotenv:** For managing environment variables.

## Setup

1. **Clone the Repository:**
   ```bash
   git clone https://github.com/mrochelle23/Homework-4-APIs-Starter.git
   cd weather-api-app
   ```

2. **Create a Virtual Environment:**
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows use `venv\Scripts\activate`
   ```

3. **Install Dependencies:**
   ```bash
   pip install -r requirements.txt
   ```

4. **Set Up Environment Variables:**
   - Create a `.env` file in the root of the project and add your OpenWeatherMap API key:
     ```env
     API_KEY=your_openweathermap_api_key
     ```

5. **Run the Application:**
   ```bash
   python app.py
   ```
   Open your browser and go to `http://127.0.0.1:5000` to access the application.

## File Structure

- **app.py:** Main application file containing the Flask app and API logic.
- **requirements.txt:** Lists the dependencies for the application.
- **.gitignore:** Specifies files and directories to ignore in Git.
- **templates/**: Contains HTML templates used for rendering pages.
  - **base.html**: Base template that includes common HTML structure.
  - **home.html**: Homepage for user input.
  - **results.html**: Displays weather results for a single city.
  - **comparison_results.html**: Displays weather comparison for two cities.
- **static/**: Contains static files such as CSS.
  - **style.css**: Styles for the application.

## Usage

1. On the home page, enter a city name and choose your desired units (Celsius, Fahrenheit, or Kelvin) to get current weather data.
2. To compare two cities, enter both city names and choose the units.
3. View results on dedicated pages showing weather conditions.

## Acknowledgements

- Developed by Make School students © 2020.
- OpenWeatherMap API for weather data.
