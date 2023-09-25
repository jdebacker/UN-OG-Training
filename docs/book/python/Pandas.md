(Chap_Pandas)=
# Pandas

ACME materials link...


# Exercises

1. Consider the following GDP per capita data (in constant 2011$, source: [Maddison Project Database](https://www.rug.nl/ggdc/historicaldevelopment/maddison/releases/maddison-project-database-2020?lang=en)):
|                | IND | MYS | USA | ZAF|
|----------------|----|----|----|----|
| 1990        |  2,087  | 8,179   | 36,982   |  6,111  |
| 2000         |  2,753  | 13,475   |  45,886  |  7,583  |
| 2010         | 4,526   |  18,574  |  49,267  | 11,319   |
| 2018 |   6,806 |  24,842  | 55,335   | 12,166   |

Create a dictionary with keys `Year`, `IND`, `MYS`, `USA`, and `ZAF` and values that are lists of the GDP per capita data for each country.  Create a DataFrame named `df` from this dictionary.  Print the DataFrame.

2. Inspect this data frame.  Print `df.head(3)`.  Print `df.tail(3)`.  Get a list of column names with the `keys` method.  Finally, use the  `describe` method to print descriptive statistics.
3. Pandas DataFrame use an index to keep track of rows.  Not the default index in `df` are integers for each row.  Let's change the index so the year is the index value. Print the updated DataFrame.
4. Let's reshape this into a long panel format with a [`MultiIndex`](https://pandas.pydata.org/docs/user_guide/advanced.html) for the columns.  The first level of the `MultiIndex` should be the country name and the second level should be the year.  The values should be the GDP per capita.  To do this, use the pivottable. Print the DataFrame.
5. Create a new variable that is the GDP growth rate from the prior period measure. Using `groupby` to find mean GDP growth rate for each country ove the sample.
6. Print a DataFrame as a table (e.g. to tex or json or md)
7. Read in a csv file as a DataFrame.  Use UN population data as an example.  Saving a DataFrame to a CSV file.
8. Creating a new variable in a DataFrame.
9.  Selecting a subset of a DataFrame. Using `.loc` and subsetting columns etc
10.  Using `merge` to join two DataFrames.  Read other UN data (e.g., fertility) and merge with data from (4)
11. Using the `plot` method
12. Replacing values, dropping, renaming columns
