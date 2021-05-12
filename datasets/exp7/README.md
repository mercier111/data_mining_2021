# Info

This Data repo contains the following datasets (in .csv format):

* 2014_Financial_Data.csv
* 2015_Financial_Data.csv
* 2016_Financial_Data.csv
* 2017_Financial_Data.csv
* 2018_Financial_Data.csv

Each dataset contains 200+ financial indicators, that are commonly found in the 10-K filings each publicly traded company releases yearly, for a plethora of US stocks (on average, 4k stocks are listed in each dataset).

Important remarks regarding the datasets:

1. Some financial indicator values are missing.so the user can select the best technique to clean each datase.
2. There are outliers, meaning extreme values that are probably caused by mistypings. Also in this case, the user can choose how to clean each dataset (have a look at the 1% - 99% percentile values).
3. The last column, class, lists a binary classification for each stock, where
   * for each stock, if the PRICE VAR [%] value is positive, class = 1. From a trading perspective, the 1 identifies those stocks that an hypothetical trader should BUY at the start of the year and sell at the end of the year for a profit.
   * for each stock, if the PRICE VAR [%] value is negative, class = 0. From a trading perspective, the 0 identifies those stocks that an hypothetical trader should NOT BUY, since their value will decrease, meaning a loss of capital.
