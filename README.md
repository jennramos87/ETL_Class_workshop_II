# Project: Data Clean

## Required Libraries
- pandas
- json
- matplotlib.pyplot

## Step by Step

1. ### Data Reading:
    - A `.jsonlines` file was read and converted into a pandas DataFrame to facilitate manipulation and analysis.

2. **Initial Exploration**:
    - The first rows of the DataFrame were visualized.
    - The dimensions of the DataFrame were obtained.
    - The original columns of the DataFrame were saved.
    - The number of null values in each column was checked.

3. **Column Removal**:
    - Completely empty columns were removed.
    - Columns with few and unnecessary data were removed.

4. **Data Type Transformation**:
    - Date columns were converted to `datetime` type.
    - Numeric columns were converted to `numeric` type.
    - Categorical columns were converted to `category` type.

5. **Dictionary Cleaning and Transformation**:
    - Columns containing dictionaries were identified.
    - Separate DataFrames were created for relevant dictionary columns (`seller_address`, `shipping`, `location`, `geolocation`).
    - Dictionary columns were removed from the original DataFrame after extracting relevant information.

6. **List Cleaning and Transformation**:
    - Columns containing lists were identified.
    - Separate DataFrames were created for relevant list columns (`sub_status`, `deal_ids`, `non_mercado_pago_payment_methods`, `variations`, `attributes`, `coverage_areas`, `descriptions`).
    - List columns were removed from the original DataFrame after extracting relevant information.

7. **New Column Creation**:
    - New columns derived from date columns were created (`year_created`, `month_created`, `year_started`, `month_started`, `year_updated`, `month_updated`).

8. **Original Column Removal**:
    - Original date columns were removed after creating the new derived columns.

9. **Data Conversion to Lowercase**:
    - Data in the `warranty` column was converted to lowercase.

10. **Data Visualization**:
     - A bar chart comparing the number of products created and updated per month was created.

11. **Data Saving**:
     - The cleaned and transformed DataFrame was saved to a CSV file.

These procedures ensure that the data is clean, structured, and ready for further analysis.
