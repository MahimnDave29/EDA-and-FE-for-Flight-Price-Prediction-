# EDA and FE of Flight Price Data
## Dataset Link: 
https://www.kaggle.com/datasets/shubhambathwal/flight-price-prediction

## 📊 Project Overview

This notebook performs exploratory data analysis (EDA) and feature engineering on a dataset of 10,683 flight records from Indian airlines in 2019. The project transforms raw flight data into ML-ready features to enable accurate price prediction modeling.

## 🎯 Objectives

- Perform comprehensive exploratory data analysis on flight pricing data
- Engineer meaningful features from datetime and categorical variables
- Handle missing values and data quality issues
- Prepare clean, structured data for machine learning models

## 📁 Dataset Information

**Dataset Size:** 10,683 flight records (2019)

**Key Features:**
- Airline (IndiGo, Air India, Jet Airways, etc.)
- Journey date and time information
- Source and destination cities
- Flight route details
- Duration and number of stops
- Additional flight information
- **Target Variable:** Price (₹1,759 - ₹79,512)

**Price Statistics:**
- Mean: ₹9,087
- Median: ₹8,372
- Standard Deviation: ₹4,611

## 🔧 Feature Engineering

### Temporal Features
- **Date extraction:** Day, Month, Year from journey date
- **Departure time:** Hour and minute components
- **Arrival time:** Hour and minute components
- **Duration breakdown:** Flight duration in hours and minutes

### Data Transformations
- Categorical encoding for airlines, sources, and destinations
- Stop count conversion (non-stop → 0, 1 stop → 1, 2 stops → 2)
- Route parsing and analysis
- Handling missing values in route information

### Cleaned Features
Final feature set includes:
- Airline, Source, Destination
- Total_Stops (numeric)
- Additional_Info
- Date, Month, Year
- Departure_hour, Departure_minute
- Arrival_hour, Arrival_minute
- Duration_hour, Duration_minute
- Price (target)

## Tech Stack
-Python (NumPy,Pandas,sklearn)

## 📈 Key Insights

- Flight prices vary significantly (44x range from min to max)
- Temporal features (date, time) are extracted for seasonality analysis
- Duration and stop count are key predictors
- Route complexity impacts pricing

## 🚀 Usage


