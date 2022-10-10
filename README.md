# EAP
Data Analysis Project – State Unemployment Rates as compared to the DOW for the selected years 2013-2022.
Project -Compare the unemployment rates of Indiana, Kentucky, Ohio, and West Virginia  (monthly percent) against the Dow Jones Industrial Average (monthly seasonally adjusted percent) for the years of 01/01/2013 through 08/01/2022.  
Objective-to see if there is a correlation between the DOW and unemployment rates for the respective states between the years of 2013 – 2022.
The following Data Sources were downloaded from FRED (https://fred.stlouisfed.org/) and combined into a single CSV file:
1.)	Dow Jones Industrial Average(DJIA) - https://fred.stlouisfed.org/series/DJIA#0
Suggested Citation:
S&P Dow Jones Indices LLC, Dow Jones Industrial Average [DJIA], retrieved from FRED, Federal Reserve Bank of St. Louis; https://fred.stlouisfed.org/series/DJIA, October 9, 2022.
2.)	Unemployment Rate in Indiana(INUR) - https://fred.stlouisfed.org/series/INUR 
Suggested Citation:
U.S. Bureau of Labor Statistics, Unemployment Rate in Indiana [INUR], retrieved from FRED, Federal Reserve Bank of St. Louis; https://fred.stlouisfed.org/series/INUR, October 10, 2022.
3.)	Unemployment Rate in Kentucky(KYUR) - https://fred.stlouisfed.org/series/KYUR
Suggested Citation:
U.S. Bureau of Labor Statistics, Unemployment Rate in Kentucky [KYUR], retrieved from FRED, Federal Reserve Bank of St. Louis; https://fred.stlouisfed.org/series/KYUR, October 10, 2022.
4.)	Unemployment Rate in Ohio(OHUR) - https://fred.stlouisfed.org/series/OHUR
Suggested Citation:
U.S. Bureau of Labor Statistics, Unemployment Rate in Ohio [OHUR], retrieved from FRED, Federal Reserve Bank of St. Louis; https://fred.stlouisfed.org/series/OHUR, October 9, 2022.
5.)	Unemployment Rate in West Virginia(WVUR) - https://fred.stlouisfed.org/series/WVUR
Suggested Citation:
U.S. Bureau of Labor Statistics, Unemployment Rate in West Virginia [WVUR], retrieved from FRED, Federal Reserve Bank of St. Louis; https://fred.stlouisfed.org/series/WVUR, October 9, 2022.


Project Components used:
1.)	Read in data from a local csv, excel file, json, or any other file type. There are many ways to do this, but using Pandas read_ functions is pretty easy.

2.)	Manipulate and clean data
a.)	Use built-in pandas or numpy functions to do things like remove 0’s and null values where they don’t belong in your dataset.
b.)	Use custom functions or lambdas to perform specific operations to clean or manipulate your data, return those values, then use them in other parts of your project.

3.)	Analyze data
a.)	Do 5 basic calculations with Pandas, like finding the sum(), median(), mean(), or mode() of a column. You could divide two columns by each other. You could multiple a column by a random integer. You could use string operations and find the most common letter in a given entry. 
b.)	Write custom functions to operate on your data. You may discover that you want to find out something particular about data that just doesn’t have a built-in Pandas function that accomplishes your goal. Maybe you want your function to read in a DataFrame, search the columns for any mention of “Cars”, then return the lowest-priced car in the column along with the mileage. This category is very open to interpretation, so any function operating on your data will work. 
4.)	Visualize data
Make 2 basic plots with matplotlib, seaborn, or any other kind of visualization library that you think looks interesting. 

5.)	Interpret your data and graphical output
a.)	Write markdown cells in Jupyter explaining your thought process and code. If you make a few plots with matplotlib, explain what the reader is seeing and why you chose to plot things that way.
b.)	If using some format other than a notebook, make sure your README explains your project.				
