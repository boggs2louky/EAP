# EAP- National (USA) Unemployment Rate, Labor Force Participation Rate, and Not In Labor Force Rate for the years 01-01-1976 - 08-01-2022.
Data Analysis Project – Calculating the National Unemployment Rate, Labor Force Participation Rate, and Not In Labor Force Rate for the years 1976-2022.
Project-Perform basic calculations using the employment level (in thousands of persons/monthly), unemployment level (in thousands of persons/monthly), and not in labor force (in thousands of persons/monthly) to determine the Unemployment Rate, Labor Force Participation, and the Not In Labor Force Rate at a national scale (USA) from the years of 1976-2022.


Definitions:

Employment Level - The civilian noninstitutional population is defined as: persons 16 years of age and older residing in the 50 states and the District of Columbia, who are not inmates of institutions (e.g., penal and mental facilities, homes for the aged), and who are not on active duty in the Armed Forces.


Unemployment Level (https://www.bls.gov/cps/cps_htgm.htm#unemployed) - The Unemployment Level is the aggregate measure of people currently unemployed in the US. Someone in the labor force is defined as unemployed if they were not employed during the survey reference week, were available for work, and made at least one active effort to find a job during the 4-week survey period.

The Unemployment Level is collected in the CPS and published by the BLS. It is provided on a monthly basis, so this data is used in part by macroeconomists as an initial economic indicator of current trends. The Unemployment Level helps government agencies, financial markets, and researchers gauge the overall health of the economy.

Note that individuals that are not employed but not actively looking for a job are not counted as unemployed. For instance, declines in the Unemployment Level may either reflect movements of unemployed individuals into the labor force because they found a job, or movements of unemployed individuals out of the labor force because they stopped looking to find a job.


Not in Labor Force - Persons who are neither employed nor unemployed are not in the labor force. This category includes retired persons, students, those taking care of children or other family members, and others who are neither working nor seeking work.


Total Population - Population includes resident population plus armed forces overseas. The monthly estimate is the average of estimates for the first of the month and the first of the following month.



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

a.)	Used built-in pandas or numpy functions to remove 0’s and null values where they don’t belong in the dataset.

b.)	Use specific operations to clean or manipulate your data, return those values, then use them in other parts of your project.


3.)	Analyze data

a.)	Do 5 basic calculations with Pandas, finding the mean() of a columns.  

b.)	Write custom functions to operate on your data. 


4.)	Visualize data
Make 2 basic plots with matplotlib, seaborn, or any other kind of visualization library that you think looks interesting. 


5.)	Interpret your data and graphical output

a.)	Write markdown cells in Jupyter explaining your thought process and code. If you make a few plots with matplotlib, explain what the reader is seeing and why you chose to plot things that way.

b.)	If using some format other than a notebook, make sure your README explains your project.				




# GDP Calculation (Based on Spending-Actual GDP) per Mentor Request (Clay Morton).

The Calculation for GDP (Based on Spending) is as follows (https://www.investopedia.com/articles/investing/051415/how-calculate-gdp-country.asp):  

GDP = (Personal consumption Expenditures + private consumption of fixed capital) + gross private investment + (government investment + government spending) + (exports – imports).



Definitions (https://www.bea.gov/help/glossary):


Personal Consumption Expenditures (PCEC) - The goods and services purchased by persons.


Consumption of fixed capital (CFC)- The charge for the using up of private and government fixed capital located in the United States. It is the decline in the value of the stock of fixed assets due to wear and tear, obsolescence, accidental damage, and aging. For general government and for nonprofit institutions that primarily serve individuals, CFC serves as a measure of the value of the current services of the fixed assets owned and used by these entities.


Gross Private Domestic Investment (GDI) - The sum of gross private domestic fixed investment, the change in private inventories, and government gross investment.


Government Consumption Expenditures and Gross Investment - The value of services produced by government, measured as the purchases made by government on inputs of labor, intermediate goods and services, and investment expenditures. It is the sum of government consumption expenditures and government gross investment.


Exports of Goods and Services - Goods and services sold by U.S. residents to foreign residents.


Imports of Goods and Services - Goods and services purchased by U.S. residents from foreign residents.


All sources came from the Federal Reserve of St. Louis FRED website (https://fred.stlouisfed.org/). The following data sources were used (all data sources are Quarterly, in Billions of Dollars, Seasonally Adjusted Annual Rate):


1.) Personal Consumption Expenditures (PCEC) - https://fred.stlouisfed.org/series/PCEC
Suggested Citation:
U.S. Bureau of Economic Analysis, Personal Consumption Expenditures [PCEC], retrieved from FRED, Federal Reserve Bank of St. Louis; https://fred.stlouisfed.org/series/PCEC, October 18, 2022.


2.) Consumption of fixed capital: Private (A024RC1Q027SBEA) - https://fred.stlouisfed.org/series/A024RC1Q027SBEA
Suggested Citation:
U.S. Bureau of Economic Analysis, Consumption of fixed capital: Private [A024RC1Q027SBEA], retrieved from FRED, Federal Reserve Bank of St. Louis; https://fred.stlouisfed.org/series/A024RC1Q027SBEA, October 18, 2022.

3.) Gross Private Domestic Investment (GDPI) - https://fred.stlouisfed.org/series/GPDI
Suggested Citation:
U.S. Bureau of Economic Analysis, Gross Private Domestic Investment [GPDI], retrieved from FRED, Federal Reserve Bank of St. Louis; https://fred.stlouisfed.org/series/GPDI, October 17, 2022.

4.) Government Consumption Expenditures and Gross Investment (GCE) - https://fred.stlouisfed.org/series/GCE#
Suggested Citation:
U.S. Bureau of Economic Analysis, Government Consumption Expenditures and Gross Investment [GCE], retrieved from FRED, Federal Reserve Bank of St. Louis; https://fred.stlouisfed.org/series/GCE, October 18, 2022.

5.) Exports of Goods and Services (EXPGS) - https://fred.stlouisfed.org/series/EXPGS#0
Suggested Citation:
U.S. Bureau of Economic Analysis, Exports of Goods and Services [EXPGS], retrieved from FRED, Federal Reserve Bank of St. Louis; https://fred.stlouisfed.org/series/EXPGS, October 17, 2022.

5.) Imports of Goods and Services (IMPGS) - https://fred.stlouisfed.org/series/IMPGS
Suggested Citation:
U.S. Bureau of Economic Analysis, Imports of Goods and Services [IMPGS], retrieved from FRED, Federal Reserve Bank of St. Louis; https://fred.stlouisfed.org/series/IMPGS, October 17, 2022.


Please also see the following link from the Bureau of Economic Analysis:  https://www.bea.gov/resources/methodologies/nipa-handbook
