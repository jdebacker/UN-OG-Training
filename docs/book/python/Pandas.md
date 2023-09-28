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
3. Pandas DataFrames use an index to keep track of rows.  Not the default index in `df` are integers for each row.  Let's change the index so the year is the index value. Print the updated DataFrame.
4. Let's reshape this into a long panel format with a [`MultiIndex`](https://pandas.pydata.org/docs/user_guide/advanced.html) for the columns.  The first level of the `MultiIndex` should be the country name and the second level should be the year.  The values should be the GDP per capita.  To do this, use the `pivottable` or `stack` methods of the DataFrame class. Please print the resulting DataFrame.
5. Create a new variable that is the growth rate in GDP  period capita from the prior period measure. To do this,  you will use `groupby` to find growth rate for each country over the sample.
6. The DataFrame object has several methods to help output a formatted table suitable for reports or presentations. Use one of these methods to print a DataFrame formatted as a [markdown](https://www.markdownguide.org/basic-syntax/) table.
7. In most cases, you are likely to use a DataFrame as a container for a large dataset, not something simple that you can enter by manually as we did above.  Pandas has [several methods](https://pandas.pydata.org/docs/user_guide/io.html) to read in data from files are various formats.  Let's use one of these methods to read in some population data from the [United Nations' World Population Prospects](https://population.un.org/wpp/).  Note that Pandas will download these data for you if you have a URL to the data file.  Here's a URL you can use for these data: [https://population.un.org/wpp/Download/Files/1_Indicators%20(Standard)/CSV_FILES/WPP2022_PopulationBySingleAgeSex_Medium_2022-2100.zip](https://population.un.org/wpp/Download/Files/1_Indicators%20(Standard)/CSV_FILES/WPP2022_PopulationBySingleAgeSex_Medium_2022-2100.zip) (Note: Zip file is about 28 MB).
8. Creating a new variable in a DataFrame.
9.  Selecting a subset of a DataFrame. Using `.loc` and subsetting columns etc
10.  Using `merge` to join two DataFrames.  Read other UN data (e.g., fertility) and merge with data from (4)
11. Using the `plot` method
12. Replacing values, dropping, renaming columns
13. Save DataFrame to disk.