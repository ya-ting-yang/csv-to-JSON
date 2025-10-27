README — Wine Data Filtering Script

### Author: Ya-Ting Yang
### Purpose: Retrieve and filter wine data by distinct fields and save the filtered results to formatted JSON files.

# Description
This Python script processes a wine dataset and filters rows based on specific conditions, including:
Type of wine (red or white)
Wine score range (e.g., between 90 and 92 points)
Region (e.g., Tuscany, Italy)
After filtering, the selected rows are saved as formatted JSON files using two methods — one with pandas and one with Python’s built-in json module.

# Workflow
Load data from CSV and inspect columns.
Identify distinct wine types using unique() and value_counts().
Filter dataset based on:
variety == 'Red Wine'
rating between 90 and 92
region == 'Tuscany, Italy'
Export results to JSON
Using pandas: to_json()
Using Python’s json.dump()
Validate that both JSON files can be successfully read.

# Output Files
filtered_wine_pandas.json → generated using pandas
data_python.json → generated using Python’s json library
Both contain all rows matching the filtering conditions.
