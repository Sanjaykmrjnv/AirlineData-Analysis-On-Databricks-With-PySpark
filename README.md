# Airline Dataset Analysis with PySpark on Databricks Community Edition

This project demonstrates how to perform data analysis on the airline dataset using PySpark on Databricks Community Edition.

## Overview

The project covers various data manipulation and analysis tasks, providing a step-by-step guide to work with PySpark DataFrames. The following operations are performed:

1. **Create DataFrame from Multiple CSV Files:**
   - Read and combine multiple CSV files (1987.csv to 2008.csv) into a single PySpark DataFrame.

2. **Define a PySpark Schema:**
   - A schema is defined for the DataFrame to ensure data consistency and type safety.

3. **View DataFrame:**
   - The initial state of the DataFrame is displayed, showing the first few rows.

4. **Count Records:**
   - The count of records in the DataFrame is returned.

5. **Select Columns:**
   - The DataFrame is narrowed down to the 'Origin,' 'Dest,' and 'Distance' columns.

6. **Filter Data:**
   - The 'where' method is used to filter data, focusing on records with a 'Year' value of 2001.

7. **Create a New DataFrame:**
   - A new DataFrame, `airlines_1987_to_2008_drop_DayofMonth`, is created by excluding the 'DayofMonth' column.

8. **Display New DataFrame:**
   - The new DataFrame is displayed for further inspection.

9. **Create 'Weekend' Column:**
   - A new column 'Weekend' is added to the DataFrame, and a new DataFrame `AddNewColumn` is created.

10. **Cast Data Type:**
    - The 'ActualElapsedTime' column is cast to an integer data type, and the schema is verified using `printSchema`.

11. **Rename 'DepTime':**
    - The 'DepTime' column is renamed to 'DepartureTime' for clarity.

12. **Drop Duplicate Rows:**
    - Duplicate rows based on 'Year' and 'Month' are removed, and a new DataFrame `DropRows` is created.

13. **Sort by Year:**
    - The data is sorted in descending order based on the 'Year' column using the `sort` method.

14. **Group Data:**
    - Data is grouped according to 'Origin' and 'Dest' columns to count occurrences and find the maximum values, respectively.

15. **Write Data in Delta Format:**
    - The processed data is saved in the Delta format for future analysis.

## Getting Started

To run this project, you will need access to Databricks Community Edition and PySpark. Make sure you have the required libraries and dependencies installed.

1. Clone this repository to your local machine.
2. Import the provided dbc file or Python script into your Databricks workspace.
3. To view the code download html file and open it in any browser.
4. Execute the code in your Databricks environment to perform the data analysis tasks.

## Contributing

Feel free to contribute to this project by creating pull requests or reporting issues. Your contributions are highly welcome!


## Acknowledgments

- The project uses the airline dataset available on Databricks Community Edition.

Happy Data Analysis!
