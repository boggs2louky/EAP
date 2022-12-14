# US Macroeconomics from 01-01-1976 - 08-01-2022


Economic Analysis Project - National (USA) Unemployment Rate, Labor Force Participation Rate, and Not In Labor Force Rate for the years 01-01-1976 - 08-01-2022. Additionally, both Nominal and Real GDP were calculated to show the variation between the two. Okun's law is discussed but no calculations were performed to assess the "law" within the project notebook. 

Project Intent - The project looks at national Unemployment Rate, Labor Force Participation Rate, and Not In Labor Force Rate for the years 01-01-1976 - 08-01-2022 on a quarterly basis. The view of these rates for the selected time period allow for insight/s into cyclical/periodic occurences where unemployment, labor force participation, and persons not in the labor force vary due to other macroeconomic variables not used in this project as well as demographic factors (population age cohorts) for the time period. Above all, it is important to remember that almost all economic data is lagging time indicator and should be viewed as a snapshot in time which is used to adjust current economic trends (regadless of scale).  Unemployment is currently at lows approximately equal to pre-covid.  Future consideration should be given to personal wages, personal credit and savings, and corporate credit and earnings providing insight into which (personal earnings vs. corporate earnings) have a greater impact upon inflation in a national economy. Additionally, population pyramids were provided to show the impact that population (in time) has upon calculations for all three rates.          


Instructions for loading project. Tested on Windows 10 22h2 VM with the following installed (in order installed):

Anaconda Version 2.3.2 (Anaconda will install Python) in VS Code you will need to set the recommended interpreter to (base)python 3.9.13 or 3.10.8 versions to allow .ipynb file to work correctly in VS Code. In VS Code be sure to set the defualt python base 3.9.13 interpreter, this will allow for all imported libraries to work within VS Code correctly for this project file. 

VS Code Version 1.72.2
	extensions installed - 	Jupyter v2022.9.1202862440
						Jupyter Cell Tags v0.1.6
						Jupyter Keymap v1.0.0
						Jupyter Notebook Renders v1.0
						Pylance v2022.10.40
						Python v2022.16.1

Restart VS Code

Download the project file as a .zip from https://github.com/boggs2louky/EAP. Extract the contents of the folder to desktop or within Downloads folder or folder location of your choice on the local machine. Open VS Code navigate to the extracted zip folder ***(C:\Users\<username here>\Downloads\EAP-main\EAP-main\data***. The following are the csv files (within the data folder) used in this notebook:
    
    Econdata =  .../EAP-main/EAP-main/data/ECONDATA.csv
    GDP = .../EAP-main/EAP-main/data/GDP.csv
    POP1980 = .../EAP-main/EAP-main/data/USA1980.csv
    POP2020 = .../EAP-main/EAP-main/data/USA2020.csv
      
    
Select the US Macroeconomics from 1976-2022.ipynb file to open in VS Code, the file should open with cells visible showing Project Title and Intro to project. You may need to set the recommended interpreter which if associated with Anaconda 2.3.2 will be base python 3.9.13 as associated with the python version installed with Anaconda and will allow the Juypter notebook kernel to be installed and to run the the ipynb project within VS Code.   

***Project was also tested on two other physical machine running Windows 10/11, with base python 3.9.13. VS Code can be installed with aformentioned dependencies/libraries (same extensions as within the VM above). A restart of VS Code may be required to allow for the installation of the jupyter notebook kernel to be installed for the purpose of running the project (jupyter notebook).***

***The instructions below are if the user computer does not have any other installation of anaconda/jupyter installed on the local machine in conjunction with VS Code. Think of it as if you have only VS Code and python installed It should be used as a last resort if the ipynb file does not load properly into VS Code by defualt. Installing a Python Library using powershell terminal. In VS Code go to Terminal -> New Terminal (Powershell) -> run the following command in powershell terminal ("pip --version" apostraphes not required). PIP version should be displayed -> run the following command "pip install pandas" (apostraphes not required). After this command is finished the respective library (pandas will be installed). You will need to do this for the following libraries:  pandas, numpy, matplotlib, plotly.express, and plotly.graph_objs should suffice.***


Data Analysis Project ??? Calculating the National Unemployment Rate, Labor Force Participation Rate, and Not In Labor Force Rate for the years 1976-2022.
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

a.)	Used built-in pandas or numpy functions to remove 0???s and null values where they don???t belong in the dataset and removed several rows from the dataset as a result of having null values.

b.)	Use specific operations to clean or manipulate your data, return those values, then use them in other parts of your project.


3.)	Analyze data

a.)	Do 5 basic calculations with Pandas, finding the mean() of a columns.  

b.)	Write custom functions to operate on your data. 
    i.) Calculate Unemployment Rate (Econdata['UNEMPLYRT'] = (Econdata['UNEMPLOY'] / Econdata['EMPLVL']) * 100)
    ii.) Calculate Labor Force Participation Rate (Econdata['LBFRCPRT'] = (Econdata['EMPLVL'] / Econdata['POPTHM']) * 100)
    iii.) Calculate Not in Labor Force Rate (Econdata['NILBRFRCRT'] = (Econdata['NINLAB'] / Econdata['POPTHM']) * 100)
    iv.) Calculate the Nominal GDP (GDP['GDPSB'] = ((GDP['PCEC'] + GDP['PRVCFC']) + GDP['GPDI'] + GDP['GCE'] + (GDP['EXPGS']-GDP['IMPGS'])))
    v.) Calculate the Real GDP (GDP['GDPR'] = GDP['GDPSB'] * 100 / GDP['GDPDEF'])

4.)	Visualize data
Made several basic plots with matplotlib for (visualization) of Unemployment Rate, Labor Force Participation Rate, Not in Labor Force Rate, Nominal GDP, Calculate the Real GDP, and demographic pyramids for 1980 and 2020 for male and female populations by age cohort. 


5.)	Interpret your data and graphical output

a.)	Write markdown cells in Jupyter explaining your thought process and code. If you make a few plots with matplotlib, explain what the reader is seeing and why you chose to plot things that way.

b.)	If using some format other than a notebook, make sure your README explains your project.				




# Nominal GDP Calculation to Real GDP Calculation per Mentor Request (Clay Morton).

The Calculation for Nominal GDP (Based on Spending) is as follows (https://www.investopedia.com/articles/investing/051415/how-calculate-gdp-country.asp):  

GDP = (Personal consumption Expenditures + private consumption of fixed capital) + gross private investment + (government investment + government spending) + (exports ??? imports). In this instance the column header GDPSB is the nominal GDP in billions of dollars.

Calculation for Real GDP = GDPSB * 100 / Index Price (GDP Implicit Price Deflator -> GDPDEF)



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

6.) Gross Domestic Product: Implicit Price Deflator (GDPDEF) - https://fred.stlouisfed.org/series/GDPDEF/
Suggested Citation:
U.S. Bureau of Economic Analysis, Gross Domestic Product: Implicit Price Deflator [GDPDEF], retrieved from FRED, Federal Reserve Bank of St. Louis; https://fred.stlouisfed.org/series/GDPDEF, October 20, 2022.

Please also see the following link from the Bureau of Economic Analysis:  https://www.bea.gov/resources/methodologies/nipa-handbook

# Okun's Law  (Unemployment and GDP Connection)

Okun's Law states that there is a relationship between Unemployment and GDP. The law predicts that for every 1% increase in unemployment there will "usually" be an associated drop of 2% in GDP.  This is interesting given the circumstances of supply chain issues and inflation as they are currently being witnessed in the economy due to COVID 19. We have to remember that many of these indicators have a lag of time in them and so what we see at the moment is in fact representative of (in this case explicitly) what has occurred over the previous three months (Quarter) in economic terms. Nonetheless, it still provides insight into our larger national economy as a whole and from my perspective is interesting to witness/research.  The following link:  https://www.investopedia.com/terms/o/okunslaw.asp provides a more detailed discussion of Okun's Law.  


