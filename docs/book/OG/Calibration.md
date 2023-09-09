(Chap_OGcalibration)=

# Calibrating the `OG-Core` model

As noted in the introduction, the `OG-Core` model must be parametrized to represent a specific country. We refer tot he process of finding parameter values that represent a specific economy as "calibration".  Because data sources for country-specific data differ, there's not a single way to calibrate all economies. We there for have created country-specific calibration packages.   Some examples of these include the [United States](https://github.com/PSLmodels/OG-USA), the [United Kingdom](https://github.com/PSLmodels/OG-UK), [South Africa](https://github.com/EAPD-DRB/OG-ZAF), [India](https://github.com/Revenue-Academy/OG-IND), and [Malaysia](https://github.com/Revenue-Academy/OG-MYS).

In this chapter, we describe the process of creating a country-specific calibration and provide exercises related to certain components of that calibration.  We will use as an example the calibraiton of `OG-Core` to South Africa, in the [`OG-ZAF`](https://github.com/EAPD-DRB/OG-ZAF) package.


# Demographics

A key feature of OG models is the ability to model effects across generations. In this way, OG models can be made to reflect realisti demographics and capture demographic trends.  Demographics are of massive importance to economic trends [add CITATIONS here].

## Exercises
1. Make a copy of `demographics.py` and modify to get UN data for specific country.
2. Plot fert rates.  Do again with alternative forecast?
3. Plot mort rates
4. Plot pop distribution over different years
5. Get pop objects and sim model SS with OG-Core defaults then your new pop objects.  Compare SS macro vars using `ogcore.output_tables.macro_table_SS`.

# Macro parameters

## Exercises
1. Use pandas datareader to get GDP series from country XXX from FRED
2. Collapse quarterly data to make annual
3. Compute average growth rate
4. Other??
# Firm Production Functions

Describe industry models, types of sources of data, etc.  SAM files... (UNU Wider)

# Earnings Processes

Earnings processes

## Exercises
1. Use `income.py` from OG-USA to retrieve e matrix.  Plot it.
2. Do approximation method of Marcelo to match a specific gini coefficient



