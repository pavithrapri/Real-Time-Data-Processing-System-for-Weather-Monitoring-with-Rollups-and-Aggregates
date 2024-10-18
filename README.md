# Real-Time-Data-Processing-System-for-Weather-Monitoring-with-Rollups-and-Aggregates


# Real-Time Weather Monitoring System

## Overview

This project implements a real-time weather monitoring system that retrieves weather data from the OpenWeatherMap API. The system provides summarized insights using rollups and aggregates, including daily weather summaries and alerting features based on user-configurable thresholds.

## Features

- Continuous data retrieval from OpenWeatherMap API for major Indian cities.
- Daily weather summaries including:
  - Average temperature
  - Maximum temperature
  - Minimum temperature
  - Dominant weather condition
- User-configurable alert thresholds for temperature and specific weather conditions.
- Visualization of historical trends and triggered alerts.
- Support for multiple weather parameters (e.g., humidity, wind speed).
- Functionality to fetch weather forecasts and generate summaries based on predicted conditions.


## Installation Instructions

### Prerequisites

- Python 3.x
- An OpenWeatherMap API key (sign up at [OpenWeatherMap](https://openweathermap.org/)).

### Dependencies

This project requires the following Python libraries:
- `requests` - For making HTTP requests to the OpenWeatherMap API.
- `pandas` - For data manipulation and analysis.
- `matplotlib` - For visualizing data.
- `smtplib` - For sending email alerts.

You can install the dependencies using pip:

```bash
pip install requests pandas matplotlib

#Setup
1.Clone the repository:
        git clone https://github.com/yourusername/weather-monitoring-system.git
        cd weather-monitoring-system
2.Create a .env file to store your OpenWeatherMap API key:
        API_KEY=your_api_key_here
3.Run the application:
        python weather_monitoring.py

Running with Docker (Optional)
To run the application in a Docker container, ensure you have Docker installed on your machine.
  Build the Docker image:
         docker build -t weather-monitoring .
   Run the Docker container:
        docker run -d -p 8080:8080 weather-monitoring


### Design Choices
API Integration: The system leverages the OpenWeatherMap API to fetch real-time weather data. This decision allows for access to a wide range of weather parameters without maintaining a local database of weather data.

Data Processing: The system processes data in real-time, rolling up and aggregating daily summaries. This ensures users receive timely and relevant weather information.

Alert Mechanism: User-configurable alerts provide flexibility, allowing users to set thresholds based on personal preferences.

Visualization: Matplotlib is used for data visualization, making it easier to interpret weather trends over time.

##Testing
To ensure the system works as intended, various test cases have been implemented:

System Setup: Verifies the connection to the OpenWeatherMap API.
Data Retrieval: Simulates API calls and checks the correctness of the response parsing.
Temperature Conversion: Tests the conversion of temperature values.
Daily Weather Summary: Validates daily rollups and aggregates.
Alerting Thresholds: Checks the functionality of the alert system when thresholds are breached.



