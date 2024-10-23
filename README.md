### Real-Time Weather Monitoring and Data Processing System

### Table of Contents
Introduction

Goal

Key Features

Project Structure

Setup Guide

API Key Configuration

Running the System

Navbar Details

Additional Features

Testing

### Introduction
This project implements a Real-Time Weather Monitoring System that processes weather data and provides analytical insights through summaries and aggregates. The system integrates with the OpenWeatherMap API to gather live weather data for various major cities in India.

# Goal
The primary goal of this system is to periodically collect weather data, compute daily weather summaries, implement alert notifications when thresholds are crossed, and display data visualizations.

# Key Features
Live Weather Data Fetching: The system pulls updated weather data every 5 minutes for these Indian metro cities:

Delhi

Mumbai

Chennai

Bengaluru

Kolkata

Hyderabad

# Data Processing:

Converts temperature readings from Kelvin to Celsius.

Produces daily weather summaries, including:

Average temperature

Maximum and minimum temperature

Dominant weather conditions

Alert System: Users can configure temperature thresholds or specific weather conditions to trigger alerts.

# Data Visualization: Displays weather summaries, historical data trends, and alerts graphically.

# Project Structure
1. app.py: The main application file responsible for routing and data handling.
2. real_time_bonus.py: Contains functions for retrieving detailed weather data.
3. visualizations/visualizations.py: Handles the generation of various weather-related visualizations.
4. data/: Stores historical weather data.
5. static/: Contains static assets like CSS and JavaScript files.
6. templates/: Houses HTML files for web page rendering.

# Setup Guide
1. Repository Cloning

git clone https://github.com/Akashn12434/Real-Time-Data-Processing-System-for-Weather-Monitoring-with-Rollups-and-Aggregates-main-Zeotap.git
cd https://github.com/Akashn12434/Real-Time-Data-Processing-System-for-Weather-Monitoring-with-Rollups-and-Aggregates-main-Zeotap
2. Virtual Environment Setup
python -m venv venv

3. Environment Activation

For Windows:
venv\Scripts\activate
4. Dependency Installation
pip install -r requirements.txt

5. Run
python app.py
Once running, you can access the application at http://localhost:5000 through your web browser.
# API Key Configuration
To interact with the OpenWeatherMap API, follow these steps to get an API key:

Go to OpenWeatherMap.
Sign up for a free API key.
Store the API key securely and reference it in the application code or as an environment variable.
Running the System
Ensure all required dependencies are installed.
Insert your API key into the relevant section of the application code or as an environment variable.

### Launch the application with the command:

python app.py
Once running, you can access the application at http://localhost:5000 through your web browser.
Navbar Details

### The navbar provides easy navigation throughout the system:

Home: Redirects to the main weather dashboard.

Live Weather: Shows up-to-the-minute weather data.

Summary: Displays daily weather reports.

Visualization: Offers graphical representations of weather data.

Feedback: A section dedicated to user feedback.

### Additional Features
Historical Weather Data: You can enhance the system to track additional metrics like humidity and wind speed and include them in aggregates and summaries.
Forecasting: Extend the application to retrieve weather forecasts and generate summaries based on future predictions.

### Testing
System Initialization: Verify that the system starts correctly and connects to the OpenWeatherMap API with a valid API key.

Weather Data Fetching: Simulate API calls at configurable intervals to ensure correct retrieval and parsing of weather data.

Temperature Conversion: Test that temperature conversions from Kelvin to Celsius (or Fahrenheit) work as intended.

Daily Summary Calculations: Simulate multiple days of weather data and verify that the summaries are calculated correctly.

Alerting System: Configure user-defined thresholds and verify that alerts are triggered when conditions are met.

To run unit tests, navigate to the tests directory.
