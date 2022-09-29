# EAP
Pandas Economic Analysis Repo for CL 

The project uses the Federal Reserve of St. Louis FRED API to view data for New Zealand's housing market.

Data Analysis Project – New Zealand Housing Market Supply versus Demand.
Project Goal- to take a look at the New Zealand Housing Market and potential impacts of lag in the construction permitting process. Demographics may be used to help illustrate elasticity of supply demand of housing. 
Project Components used:
1.)	Read Data
Use an API to pull in data, FRED API. The most common library for this is “requests”, while pulling the data itself is usually pretty easy, sometimes going through the specific API documentation can be kind of complicated. The FRED API is imported and requires the user to sign up for an API key, this project requires that the end user sign up and obtain their own API key to view the project and associated data.

2.)	Manipulate and clean data
a.)	Use built-in pandas or numpy functions to do things like remove 0’s and null values where they don’t belong in your dataset.
b.)	Use custom functions or lambdas to perform specific operations to clean or manipulate your data, return those values, then use them in other parts of your project.

3.)	Analyze data
a.)	Do 5 basic calculations with Pandas, like finding the sum(), median(), mean(), or mode() of a column. You could divide two columns by each other. You could multiple a column by a random integer. You could use string operations and find the most common letter in a given entry. 
b.)	Write custom functions to operate on your data. You may discover that you want to find out something particular about data that just doesn’t have a built-in Pandas function that accomplishes your goal. Maybe you want your function to read in a DataFrame, search the columns for any mention of “Cars”, then return the lowest-priced car in the column along with the mileage. This category is very open to interpretation, so any function operating on your data will work. (This will be used with deconstructing the CPI (Consumer Price Index as established by each data set from the base year)

4.)	Visualize data
Make 2 basic plots with matplotlib, seaborn, or any other kind of visualization library that you think looks interesting. 

5.)	Interpret your data and graphical output
a.)	Write markdown cells in Jupyter explaining your thought process and code. If you make a few plots with matplotlib, explain what the reader is seeing and why you chose to plot things that way.
b.)	If using some format other than a notebook, make sure your README explains your project.	