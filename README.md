# EAP- National (USA) Unemployment Rate and Labor Force Participation
Data Analysis Project – Calculating the National Unemployment Rate and Labor Force Participation Rate for the years 1976-2022.
Project-Perform basic calculations using the employment level (in thousands of persons/monthly), unemployment level (in thousands of persons/monthly), and not in labor force (in thousands of persons/monthly) to determine the Unemployment Rate and Labor Force Participation at a national scale (USA) from the years of 1976-2022.

The following Data Sources were downloaded from FRED (https://fred.stlouisfed.org/) and combined into a single CSV file:
1.)	Employment Level (CE16V) - https://fred.stlouisfed.org/series/CE16OV
Suggested Citation: U.S. Bureau of Labor Statistics, Employment Level [CE16OV], retrieved from FRED, Federal Reserve Bank of St. Louis; https://fred.stlouisfed.org/series/CE16OV, October 12, 2022.

2.)	Unemployment Level (UNEMPLOY) - https://fred.stlouisfed.org/series/UNEMPLOY/ 
Suggested Citation: U.S. Bureau of Labor Statistics, Unemployment Level [UNEMPLOY], retrieved from FRED, Federal Reserve Bank of St. Louis; https://fred.stlouisfed.org/series/UNEMPLOY, October 12, 2022.

3.)	Not in Labor Force (LNS15000000) - https://fred.stlouisfed.org/series/LNS15000000#0
Suggested Citation: U.S. Bureau of Labor Statistics, Not in Labor Force [LNS15000000], retrieved from FRED, Federal Reserve Bank of St. Louis; https://fred.stlouisfed.org/series/LNS15000000, October 11, 2022.

4.) Total Population of USA (POPTHM) - https://fred.stlouisfed.org/series/POPTHM
Suggested Citation: U.S. Bureau of Economic Analysis, Population [POPTHM], retrieved from FRED, Federal Reserve Bank of St. Louis; https://fred.stlouisfed.org/series/POPTHM, October 13, 2022.  



Project Components used:

1.)	Read in data from a local csv.


2.)	Manipulate and clean data

a.)	Used built-in pandas or numpy functions to remove 0’s and null values where they don’t belong in your dataset.
b.)	Use specific operations to clean or manipulate your data, return those values, then use them in other parts of your project.


3.)	Analyze data

a.)	Do 5 basic calculations with Pandas, finding the mean() of a columns.  
b.)	Write custom functions to operate on your data. 


4.)	Visualize data
Make 2 basic plots with matplotlib, seaborn, or any other kind of visualization library that you think looks interesting. 


5.)	Interpret your data and graphical output

a.)	Write markdown cells in Jupyter explaining your thought process and code. If you make a few plots with matplotlib, explain what the reader is seeing and why you chose to plot things that way.
b.)	If using some format other than a notebook, make sure your README explains your project.				
