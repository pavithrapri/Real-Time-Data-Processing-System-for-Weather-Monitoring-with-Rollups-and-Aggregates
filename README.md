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

## Codebase

The complete codebase is hosted on GitHub. You can access it [here](https://github.com/yourusername/weather-monitoring-system).

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
