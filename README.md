# NYC Yellow Taxi Trip Data - Exploratory Data Analysis (2023)

![Python](https://img.shields.io/badge/Python-3.10%2B-blue)
![Pandas](https://img.shields.io/badge/Pandas-2.x-green)
![GeoPandas](https://img.shields.io/badge/GeoPandas-1.x-orange)
![License](https://img.shields.io/badge/License-MIT-yellow)

## Project Overview
This project performs a comprehensive **Exploratory Data Analysis (EDA)** on the 2023 New York City Yellow Taxi trip records.  

The goal is to uncover patterns and insights that can help taxi operators:
- Optimize operations and fleet allocation
- Maximize revenue
- Improve passenger experience

**Dataset**: Official TLC Yellow Taxi Trip Records (2023)  
**Sample Size**: ~1.68 million trips (intelligent 5% hourly sampling)

---

## Key Features & Analysis

### 1. Data Preparation & Cleaning
- Loaded and combined 12 monthly Parquet files
- Applied stratified sampling (5% of trips per hour per day) to handle large volume
- Fixed negative monetary values, missing values, and logical errors
- Handled outliers using IQR + logical rules (zero distance + high fare, invalid payment types, etc.)
- Cleaned passenger count, RatecodeID, and airport fee columns

### 2. Temporal Analysis
- Hourly pickup distribution (peak hours identified)
- Day-of-week patterns (weekday vs weekend)
- Monthly pickup and revenue trends
- Night-time (11 PM – 5 AM) vs Day-time analysis

### 3. Financial Analysis
- Monthly and quarterly revenue trends
- Relationship between trip distance and fare amount
- Correlation of fare with trip duration and passenger count
- Tip amount vs trip distance analysis
- Average fare per mile by hour, day, vendor, and distance tiers
- Tip percentage analysis across distance, passenger count, and pickup hour

### 4. Geospatial Analysis
- Merged trip data with official NYC Taxi Zone shapefile
- Created choropleth maps showing trip volume by zone
- Identified top pickup and dropoff zones
- Analyzed pickup/dropoff ratios and night-time high-traffic zones

### 5. Operational Insights
- Slowest routes by average speed
- High-demand zones during different times of day
- Passenger count variation across hours, days, and zones
- Frequency of extra charges and surcharges

---

## Tech Stack
- **Language**: Python
- **Libraries**: Pandas, NumPy, Matplotlib, Seaborn, GeoPandas
- **Data Format**: Parquet
- **Tools**: Jupyter Notebook / Google Colab

---

## Project Structure
