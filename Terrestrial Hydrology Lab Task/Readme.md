# Hydrology Research Project

## Overview

This repository contains the solutions to two hydrology-related questions. The solutions involve working with shapefiles, CSV data, and NASA GPM rainfall data using Python programming. The repository includes two Jupyter notebooks (`Task1.ipynb` and `Task2.ipynb`) which provide the code and detailed reasoning for each step. Screenshots of the steps are documented in a Word file.

## Author
- **Name:** Arjun Adhikari
- **Date:** June 17, 2024
- **Education:** Third-year Civil Engineering Student at Pulchowk Campus

## Contents

- `Task1.ipynb`: Solution to Question 1
- `Task2.ipynb`: Solution to Question 2
- `file1.zip`: Contains the shapefile and CSV table for Question 1
- `file2.zip`: Contains the point shapefile for Question 2
- `Documentation.docx`: Screenshots of the steps documented in a Word file

## Question 1: Merging Wind Speed Data with Shapefile

### Problem Statement
The `file1.zip` file contains a shapefile and a CSV table. The shapefile has a column named `COMID`, which is the notation of the wind speed gauge station. The wind speed values are present in the CSV file. Merge them such that the wind speed observations are added in a column corresponding to their `COMID` station numbers in the shapefile.

### Solution
The solution is provided in the `Task1.ipynb` Jupyter notebook. The notebook demonstrates how to use Python to merge the wind speed data with the shapefile. The steps are clearly commented for understanding.

### Steps
1. **Extract the files**: Unzip the `file1.zip` to get the shapefile and CSV file.
2. **Load the shapefile**: Use `geopandas` to load the shapefile.
3. **Load the CSV data**: Use `pandas` to load the CSV file containing wind speed data.
4. **Merge the data**: Merge the CSV data with the shapefile data based on the `COMID` column.
5. **Save the result**: Save the updated shapefile.

## Question 2: Generating Rainfall Time Series Data

### Problem Statement
NASA GPM provides a 30-minute temporal resolution and 0.1-degree spatial resolution rainfall data for the entire world in various formats. Generate the time series data for the rainfall data for the period of 2019-01-01 to 2020-12-31 for the location indicated in the point shapefile provided in `file2.zip`.

### Solution
The solution is provided in the `Task2.ipynb` Jupyter notebook. The notebook demonstrates how to use Python to extract rainfall time series data for the specified location. The steps are clearly commented for understanding.

### Steps
1. **Extract the files**: Unzip the `file2.zip` to get the point shapefile.
2. **Load the point shapefile**: Use `geopandas` to load the point shapefile.
3. **Download rainfall data**: Fetch the rainfall data from NASA GPM.
4. **Extract time series data**: Use the `precipitationCal` variable to generate the time series data for the specified period.
5. **Save the result**: Save the extracted time series data.

## Learning Experience

This project helped in applying Python programming skills to solve real-world hydrology problems. It enhanced problem-solving capacity and provided experience in working with geospatial data and time series analysis. The dataset comprising two years of rainfall data can be analyzed to identify patterns and create training sets for machine learning models.
