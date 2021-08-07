The dataset contains data from January 4 until July 31. Each row describes the COVID-19 report for one day in one specific country (the first few rows show only China because the virus was only present in China at that time).

For each row, we have the following data points:

- `Date_reported`: The date when the data was reported in year-month-day format.
- `Country`: The country to which the report corresponds.
- `New_cases`: The number of new cases reported for that date and for that country.
- `Cumulative_cases`: The number of total cases up to that date in that country.
- `New_deaths`: The number of new deaths reported for that date and for that country.
- `Cumulative_deaths`: The number of total deaths up to that day in that country.

The rows in our dataset are listed in time order, starting with January 4 and ending with July 31. We call a series of data points that is listed in time order a **time series**.

Typically we visualize time series with line graphs. The time values are always plotted, by convention, on the x-axis.

Let's read in our dataset in the following exercise.



1. Import the pandas module as pd.
2. Read in the WHO_time_series.csv file using the pd.read_csv() function. Assign the resulting DataFrame to a variable named who_time_series.
3. Transform the Date_reported column to a datetime data type using `pd.to_datetime()`(https://pandas.pydata.org/pandas-docs/stable/reference/api/pandas.to_datetime.html). Assign the DataFrame with the modified column back to the who_time_series variable.
4. Print the first and the last five rows and examine the data points. Be sure to specify print().
5. Print information about the dataset using the DataFrame.info() method. How many rows and columns does the dataset have? Do you see any missing values?
