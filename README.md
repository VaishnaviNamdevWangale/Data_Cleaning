1. Import Required Libraries
      Imports the pandas library for data manipulation.
      Disables warnings to keep the output clean.


2. Load the Dataset
      Loads the CSV file named data.csv into a DataFrame.
      Prints the entire dataset to inspect all rows.


3. Get DataFrame Info
      Displays column names, data types, null values, and memory usage.
      Helps you understand the structure of your data.


4. Handle Missing Values by Dropping Rows
      Removes rows that contain any missing values (NaN).
      Shows the cleaned DataFrame and its structure.


5. Fill Missing Values with a Constant (All Columns)
      Replaces all missing values in the DataFrame with 130.


6. Fill Missing Values in a Specific Column
      Targets only the Calories column for filling missing values with 130.
      

7. Fill Using the Mean
      Calculates the mean of the Calories column.
      Attempts to fill missing values (but doesn’t apply without inplace=True).


8. Fill Using the Median
      Replaces missing values in Calories with the median.


9. Fill Using the Mode
      Fills missing values in Calories with the most frequent value.


10. Detect and Remove Duplicates
      Checks for duplicate rows.
      Removes duplicates and updates the DataFrame.


11. Correlation Matrix
      Calculates correlations between numerical columns.
      Helps identify relationships between variables.


