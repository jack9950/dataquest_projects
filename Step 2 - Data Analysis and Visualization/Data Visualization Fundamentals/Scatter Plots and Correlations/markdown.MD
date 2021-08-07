Each row describes the number of bike rentals for a single day and the corresponding weather. The data spans a period of two years (January 1, 2011 – December 31, 2012). Here are some of the columns we'll be focusing on:

- `dteday`: date in year-month-day format.
- `temp`: normalized temperature in Celsius (1 is the maximum value, and it's equivalent to 41 Celsius degrees).
- `atemp`: normalized feeling temperature in Celsius (1 is the maximum value, and it's equivalent to 50 Celsius degrees).
- `hum`: normalized humidity.
- `windspeed`: normalized wind speed.
- `casual`: the number of casual (non-registered) people who rented a bike that day.
- `registered`: the number of registered people who rented a bike that day (registered people bought a membership).
- `cnt`: the total number of people who rented a bike (casual plus registered).

Researcher Hadi [Fanaee-T](https://www.researchgate.net/profile/Hadi-Fanaee-T) collected the dataset, and you can download it from the [UCI Machine Learning Repository](https://archive.ics.uci.edu/ml/datasets/bike+sharing+dataset).

Let's read in the dataset using pandas. On the next screen, we'll start exploring the dataset using visualization.



1. Import the `pandas` module as `pd`.
2. Read in the `day.csv` file using the `pd.read_csv()` function. Assign the result to a variable named `bike_sharing`.
3. Examine the first and the last five rows.
4. Display information about the dataset using the `DataFrame.info()` method. How many rows and columns does this dataset have? Do you see any missing values?
