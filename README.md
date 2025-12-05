Repository Name: `MajiNdogo_Agriculture_Analysis`

Description: `Exploratory Data Analysis and Cleaning of Maji Ndogo's agricultural data. This repository contains Python code using Pandas and SQL to import, clean, and analyze farm survey data, identifying optimal conditions for various crop types and fertile soil zones.`

# README.md

# Maji Ndogo Agriculture Analysis

This repository houses the code and analysis for understanding agricultural practices in Maji Ndogo. The project focuses on leveraging data to make informed decisions about crop placement, soil management, and overall farming automation.

## Project Overview

Maji Ndogo presents a diverse and challenging agricultural landscape. This analysis aims to: 
- Import and integrate agricultural data from an SQLite database into a single Pandas DataFrame.
- Clean and preprocess the data to handle inconsistencies and errors.
- Conduct exploratory data analysis to uncover patterns related to crop distribution, soil fertility, climate, and geographic features.
- Identify optimal conditions for specific crops (e.g., tea, wheat) based on rainfall, elevation, temperature, and soil type.

## Data Sources

The primary data source is an SQLite database (`Maji_Ndogo_farm_survey_small.db`) containing several tables related to:
- **Geographic features**: Field_ID, Elevation, Latitude, Longitude, Location, Slope
- **Weather features**: Field_ID, Rainfall, Min_temperature_C, Max_temperature_C, Ave_temps
- **Soil and crop features**: Field_ID, Soil_fertility, Soil_type, pH
- **Farm management features**: Field_ID, Pollution_level, Plot_size, Chosen_crop, Annual_yield, Standard_yield

## Key Analyses Performed

1.  **Data Integration**: SQL queries are used to join multiple tables into a unified Pandas DataFrame.
2.  **Data Cleaning**: Addresses swapped column names, corrects spelling errors in crop types, and rectifies illogical negative elevation values.
3.  **Crop Distribution Analysis**: Explores the mean rainfall and elevation for specific crops to understand their preferred growing conditions.
4.  **Soil Fertility Analysis**: Groups data by soil type to identify the most fertile regions.
5.  **Climate and Geography Influence**: Analyzes the impact of elevation, temperature, and rainfall on crop yields.
6.  **Top Crop Identification**: Determines the crop with the highest number of fields exhibiting above-average standard yield.
7.  **Advanced Filtering**: Identifies ideal growing conditions for top-performing crops based on yield, temperature, and pollution levels.

## Technologies Used

-   Python
-   Pandas (for data manipulation and analysis)
-   SQLAlchemy (for database interaction)
-   SQLite (database)

## How to Use

To replicate this analysis:
1.  Ensure you have the `Maji_Ndogo_farm_survey_small.db` file in your working directory.
2.  Install the required Python libraries:
    ```bash
    pip install pandas sqlalchemy
    ```
3.  Run the Python script or Jupyter Notebook containing the provided code cells.

## Contribution

Feel free to fork this repository, suggest improvements, or raise issues. Any contributions to enhance the data cleaning, analysis, or visualization techniques are welcome.
