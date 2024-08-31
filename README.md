# PySpark Data Exploration System

## Overview

This PySpark-based system is designed to perform basic data exploration on CSV files. The system is generic and can work with any CSV file, outputting structured JSON data containing the exploration results.

## Features

- **Data Cleaning**: Initial sanity check for the csv data.
- **Missing Value Calculation**: Computes the number of missing values in each column.
- **Column Categorization**: Categorizes columns into categorical, discrete, continuous, and text.
- **Statistics Extraction**: Extracts distinct values, frequencies, min/max values, histograms, and word counts based on the column category.

## Usage

1. **Load CSV File**: The system reads a CSV file into a PySpark DataFrame.
2. **Missing Value Calculation**: The system calculates and displays the missing values for each column.
3. **Column Categorization**: Columns are categorized into the appropriate types based on heuristics.
4. **Statistics Extraction**: Extracts relevant statistics based on the category of the column.
5. **Output**: The results are saved as a JSON file.

## How to Run

1. Set up your environment with Python and PySpark.
2. Execute the script `data_exploration.py` with the path to your CSV file.
3. The output will be saved as `output.json`.

## Example

```bash
spark-submit data_exploration.py path_to_csv_file.csv
