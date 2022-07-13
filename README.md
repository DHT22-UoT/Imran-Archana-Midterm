
***NOTE:*** due to improper management of version control, excess commits involving deletion files are present

# Files

**station.csv**; Contains data that represents a station where users can pick up or return bikes.

**trips.csv**; Data about individual bike trips.

**weather.csv**; Data about the weather on a specific day for certain zip codes/cities.

# Branches:
## trip-EDA (Archana)
- Conduct an EDA on Trip dataset
- **main files:** trip-eda.R
  - Produces plots and summaries of data

## weather-EDA (Imran)
- Conduct an EDA on Trip dataset
- **main files:** weather-eda.R
  - Produces plots and summaries of data
  - Produces weather_processed.rds that contains adjustments to events, precipitation inches, and zip code variables

## cancelled_trips (Archana)
- Remove trips with duration less than 2 minutes
- **main files:** cancelled_trips.R
  - Produces trips_2minutes.RDS that contains trips that are exclusively longer than 2 minutes

## outliers (Archana)
- Identifies and removes outliers
- **main files:** Outliers.R
  - Produces trips_no_outliers.rds that contains trip data with no outliers
  - Produces weather_no_outliers.rds that contains weather data with no outliers

## rush-hour (Imran)
- Determines highest volume rush hours on weekdays
- Determines 10 most frequent starting stations and ending stations during the rush hours
- Determines 10 most frequent starting stations and ending stations during the weekends
- **main files:** rush_hours.R

## avg_utilization (Archana)
- Determines the average utilization of bikes for each month (total time used/total time in month)
- **main files:** avg_utilization.R

## weather-conditions (Imran)
- Visualizes correlation between distance of bike rides and different weather metrics
- **main_files:** trip_weather_joined.R
  - Joins trip to station using station IDs as join condition
  - Joins weather to trip+station using date and city as join condition

