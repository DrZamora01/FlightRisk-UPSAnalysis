# FlightRisk-UPSAnalysis
Examining UPS aircraft damage incidents. Focuses on identifying trends across different aircraft models (Boeing, Airbus, MD-11) and exploring patterns related to aircraft reliability and operational issues.

# UPS Aircraft Incident Analysis

## Project Overview
This project analyzes UPS aircraft incident data for Boeing, MD-11, and Airbus models. It uses Python for data cleaning, visualization, and SQLite database integration to explore trends and patterns in incident reports.

## Features
- Data cleaning and preprocessing  
- SQLite database integration for storing and querying incident and aircraft data  
- Visualizations:
  - Incident counts by aircraft model
  - Top flight phases by aircraft type
  - Damage type distribution by aircraft type
  - Percentage comparison of incidents by aircraft type
- Functions for bucketing pilot hours and generating percentage-based comparisons

## Data Source
The incident data was obtained from the **FAA Accident and Incident Data System (AIDS)** public records.  

The dataset includes:
- Incident details (location, phase of flight, damage type, etc.)
- Aircraft make, model, and type
- Pilot flight time

The data was cleaned and filtered to include only UPS-operated aircraft of type Boeing, Airbus, and MD-11.

## How to Use the `requirements.txt`
The `requirements.txt` file lists all the Python packages needed to run this project.

1. **Create and activate a virtual environment:**
   python -m venv airplane
   source airplane/Scripts/activate      # Windows
   # or
   source airplane/bin/activate          # Mac/Linux

2. **Install the required packages:**
pip install -r requirements.txt

3.**Start Jupyter Notebook:**
jupyter notebook

4.**Open and run:**
notebooks/UPS_Analysis_main.ipynb

## SQL Usage
SQLite is used to store cleaned aircraft and incident data, enabling queries to combine information from multiple tables for analysis.

## Future Improvements
Add fleet size data for normalized incident rates

Integrate weather data for additional context

Use predictive modeling for risk assessment