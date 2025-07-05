1. Import Required Libraries
      import pandas as pd
      import warnings 
      warnings.filterwarnings("ignore")
      Imports the pandas library for data manipulation.
      Disables warnings to keep the output clean.


2. Load the Dataset
      df = pd.read_csv("data.csv")
      print(df.to_string())
      Loads the CSV file named data.csv into a DataFrame.
      Prints the entire dataset to inspect all rows.


3. Get DataFrame Info
      df.info()
      Displays column names, data types, null values, and memory usage.
      Helps you understand the structure of your data.


4. Handle Missing Values by Dropping Rows
      new_df = df.dropna()
      print(new_df.to_string())
      new_df.info()
      Removes rows that contain any missing values (NaN).
      Shows the cleaned DataFrame and its structure.


5. Fill Missing Values with a Constant (All Columns)
      df.fillna(130, inplace=True)
      df.info()
      Replaces all missing values in the DataFrame with 130.


6. Fill Missing Values in a Specific Column
      df["Calories"].fillna(130, inplace=True)
      df.info()
      Targets only the Calories column for filling missing values with 130.
      

7. Fill Using the Mean
      x = df["Calories"].mean()
      df["Calories"].fillna(130)  # Note: this doesn't modify df without inplace=True
      df.info()
      Calculates the mean of the Calories column.
      Attempts to fill missing values (but doesn’t apply without inplace=True).


8. Fill Using the Median
      x = df["Calories"].median()
      df["Calories"].fillna(x, inplace=True)
      df.info()
      Replaces missing values in Calories with the median.


9. Fill Using the Mode
      x = df["Calories"].mode()[0]
      df["Calories"].fillna(x, inplace=True)
      df.info()
      Fills missing values in Calories with the most frequent value.


10. Detect and Remove Duplicates
      print(df.duplicated())
      df.drop_duplicates(inplace=True)
      df.info()
      Checks for duplicate rows.
      Removes duplicates and updates the DataFrame.


11. Correlation Matrix
      df.corr()
      Calculates correlations between numerical columns.
      Helps identify relationships between variables.


