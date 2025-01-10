<h1 align="center"> Weather Dashboard </h1> <br>

<p align="center">
  30 Days of DevOps. Day 1.
</p>


<!-- START doctoc generated TOC please keep comment here to allow auto update -->
<!-- DON'T EDIT THIS SECTION, INSTEAD RE-RUN doctoc TO UPDATE -->
## Table of Contents
- [Introduction](#introduction)
- [Features](#features)
- [Build Process](#build-process)
- [Acknowledgments](#acknowledgments)

<!-- END doctoc generated TOC please keep comment here to allow auto update -->


## Introduction
This project is the first in the 30 days of DevOps challenge, where we will spend the next 30 consecutive days building projects to enhance and showcase our skillsets. This project demonstrates the following principles:
- External API Integration (OpenWeather API)
- Cloud Storage (AWS S3)
- Infrastructure as Code
- Version Control (Git)
- Python Development
- Error Handling
- Environment Management


## Features
* Fetch accurate, real-time weather data.
* Dashboard data displays the city, current temperature, humidity levels, conditions, etc.
* Data is automatically saved to the cloud (S3) for easy, secure storage.
* Can track weather for multiple cities.
* Timestamped data for historical tracking.

<p align="center">
  <img src = "https://rodger-project-images.s3.us-east-1.amazonaws.com/Screenshot+2025-01-09+235213.png" width=400>
  <h6 align="center">Example output</h6>
</p>

## Project Structure
weather-dashboard/
├── src/
│ ├── init .py
│ └── weather_dashboard.py
├── tests/
│ └── test_weather_dashboard.py
├── data/
│ └── .gitkeep
├── .env
├── .gitignore
├── requirements.txt
└── README.md


## Build Process

## Features
- Fetches real-time weather data from OpenWeather API
- Supports multiple Florida cities (Miami, Orlando, Tampa, Ocala)
- Stores weather data in AWS S3
- Tracks temperature, feels like temperature, humidity, and weather conditions

## Prerequisites
- Python 3.8 or higher
- AWS account with appropriate permissions
- OpenWeather API key
- AWS CLI installed and configured

## Setup Instructions

1. Clone the repository:
```bash
git clone https://github.com/ShaeInTheCloud/30days-weather-dashboard.git
cd 30days-weather-dashboard
```

2. Create and activate virtual environment:
```bash
python -m venv venv
source venv/bin/activate
```

3. Install dependencies 
```bash
pip install -r requirements.txt
```

4. Configure environment variables. Make sure to put your API keys into your .env file

5. Configure AWS credentials
```bash
aws configure
```

6. Run the application
```bash
python3 src/weather-dashboard.py
```

**Keys**: The `OPENWEATHER_API_KEY` in `src/weather_bashboard.py` must be set in your own env. You can generate your own free API key by registering an account on [OpenWeatherMap](https://home.openweathermap.org/) to generate an API key automatically. You can save your key in your .env file by using the `echo 'OPENWEATHER_API_KEY=your-api-key-goes-here' >> .env` command in your terminal.


## Acknowledgments
Thanks to [Shae](https://www.github.com/ShaeInTheCloud) for inspiring this project.
