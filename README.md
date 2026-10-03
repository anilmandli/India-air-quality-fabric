# India air quality Intelligence Platform fabric
This project builds an automated Air Quality Intelligence Platform using real, messy data from Indian cities.

## Problem Statement 
Air quality in major Indian cities fluctuates sharply with urbanization and seasonal weather, affecting urban health and environmental monitoring. However, raw PM2.5 and PM10 readings are spread across many monitoring stations and frequently contain missing values, outliers, and late-reporting intervals, which makes them hard to compare across cities.

This project ingests hourly OpenAQ sensor data and Open-Meteo weather data into Microsoft Fabric (Lakehouse and Warehouse). An automated data quality framework validates incoming readings, and idempotent Bronze-to-Gold batch pipelines turn them into standardized CPCB Air Quality Indices. The result lets city planners and analysts track seasonal pollution trends and assess station reliability across major Indian cities.

## Business Queations
## Business Questions Solved

| # | Question | Needed from Data | Where it Appears |
|---|---|---|---|
| 1 | Which cities exceed the "Poor" AQI threshold (>200) most frequently over the past 12 months? | Daily AQI per city | India overview |
| 2 | How does PM2.5 concentration vary across months for each major city? | Monthly PM2.5 | India overview |
| 3 | What are the recent daily AQI trends across major Indian metros? | Last 60 days of daily AQI | India overview |
| 4 | How do hourly PM2.5 levels correlate with weather metrics (temperature, wind speed)? | PM2.5 + weather, hourly | City deep-dive |
| 5 | What is the data completeness and sensor reliability rate across monitoring stations? | Expected vs received readings | Data quality |
| 6 | What are the hourly and weekday pollution patterns specifically for Ahmedabad? | Hourly PM2.5, Ahmedabad | City deep-dive |

Ahmedabad has PM2.5 only from Maninagar and PM10 only from Rakhial (a different station)

## Data source 

## Architecture

## Tech Stack

## Project Status / Roadmap
