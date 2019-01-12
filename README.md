# UCB_Project1_team
Authors: Sean Lane, Casey Hill, Grace Hsu

Project 1 Proposal
Collaborators: 
	Sean Lane
	Grace Hsu
	Casey Hill

Project Title: Correlation between Stock Price and Housing Prices Near Company Headquarters

Synopsis
	
Could the housing market be predicted by the stock market? From the Forbes Fortune 2017 data, Business Insider mapped out the biggest company (by revenue) headquartered in each state. This led to the hypothesis that these Fortune 1000 company’s stock affect the housing prices in their headquarters’ city. Twenty companies (five from each category: Tech, Finance, Retail, Other) were chosen at random from the list provided by Business Insider to evaluate if there are relationships between company stock prices and housing prices, and related questions as the data admits.

Questions Posed for Research

Hypothesis: As stock fluctuates for a company, the city in which they are headquartered will see a fluctuation in housing prices.
1.	What periods (ie. monthly, quarterly) are stock price changes and housing market correlated from years 2005 to 2015? Are they correlated?
a.	Is there a difference in pricing between housing sub-categories (House, Condo, Apartment)?
b.	Observing stock changes to the company’s headquarter state housing prices.
2.	If there is correlation between stock and housing prices, what level of change can be expected from this single variable?
3.	What correlation can we find between our hypothesis and the sub-category of the company? (Industrial/Tech, Finance, Retail, Other)

Execution

Analysis will be completed with the following parameters:

1.	Companies
Five top companies per industry (Industrial/Tech, Finance, Retail, Other) were chosen at random from the list provided by Forbes Fortune 1000 for a total of twenty companies. All companies will be unique based on the state that the headquarters are based. While some companies will have multiple offices or sites, we are basing the housing market impact of only the main headquarters’ city. This is based on the assumption that the company’s largest impact on employment and economy will be in the town they are headquartered.


2.	Stock Price
	Analysis will be performed on the company’s stock based on their monthly close price over the course of 10 years (2005-2015).

3.	House Prices
Housing prices will be evaluated based on the median house price in the city for each company’s headquarters. The median house price based on the dates of stock data will be used. Since stock data is the variable that will fluctuate based on high and low data points, stock dates will be used to pull median house prices in the given areas. 

Resources

The following APIs will be utilized to gather stock and housing data:
•	https://www.quandl.com/tools/api
•	API with stock data for companies listed on any stock exchange. This data will be used to pull information on the selected companies and their stock information
•	https://blog.quandl.com/api-for-housing-data
•	API with housing information from 2006 to present. Neighborhood and city information based on the selected companies headquarter cities will be used.
Article from Business Insider:
•	https://www.businessinsider.com/biggest-company-almost-every-us-state-map-2018-5


Considerations

The data might return a delayed reaction to stock price and housing price. If this is the case, data prior to the housing prices will be pulled so stock that might affect future prices may be observed. Analysis will be on-going. 

The data set will be analyzed in the following order:

1.	Find company name, stock ticker name and headquartered city
a)	Data will be manually researched and added to a csv file
b)	Data will be formatted to pull correctly from the respective APIs
2.	Pull relative stock ticker information
a)	Will create dataframe around stock price dates and information. Index will be len(dataframe), and columns will be determined based on information we acquire from APIs
3.	Pull housing price data based on stock dates for each companies neighborhood
a)	Use zillow information to find MEDIAN house price in city the company is headquartered. We will find information based on the dates we create with stock information, or possibly monthly data. 
4.	Visualize Data
a)	Data may require multiple plots based on factors we do not know (sub-category, stock price average, overall drop or increase in stock price, etc.).
b)	Data plots will be determined as data is collected and combined for ease of viewing analysis.
