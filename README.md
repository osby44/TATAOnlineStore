## Background

An online retail store has been performing well and the management wants to analyse what the major contributing factors are to the revenue so they can strategically plan for next year.
Management intends to expand the business and is interested in seeking guidance into areas that are performing well so they can keep a clear focus on what’s working. They would also like to view different metrics based on the demographic information that is available in the data.

### Project Goal

To draft the relevant analytics and insights that would help evaluate the current business performance and suggest metrics that would enable them to make the decision on expansion.

### Questions

#### *Question 1*

How was the monthly sales trend for year 2011? The CEO is interested in viewing the seasonal trends and wants to dig deeper into why these trends occur. This analysis will be helpful for the CEO to forecast for the next year.

#### *Question 2*

Excluding United Kingdom, which are the top 10 countries that are generating the highest revenue? the CMO is interested in viewing the quantity of products sold along with the revenue generated. The CMO does not want to have the United Kingdom in this visual.

#### *Question 3*

In a bid to ensure customers remain satisfied with their products, the CMO wants to know the customers generating the highest revenues. So, who are the top 10 customers by revenue?

#### *Question 4*

From a spatial view, which regions command the greatest demand for the company’s products? This is necessary as the CEO plans to initiate an expansion strategy that will allow the company to target these areas and generate more business for the regions.

### Data cleaning

Removed any records that have negative quantities and unit price, as these records needed to be removed in order to provide helpful analysis. Also removed blank rows.

### Data modeling

The dataset does not have a revenue/total sales column which is necessary for the analysis. We added a revenue column by using the DAX expression: 
Revenue = 'Online Retail'[Quantity] * 'Online Retail'[UnitPrice]

### Analysis & Visualizations

#### Question 1
![Screenshot (105)](https://github.com/osby44/TATAOnlineStore/assets/141450625/5f8ccb7a-1827-4383-9a2d-e15d9ed2c34a)

#### Question 2
![Screenshot (106)](https://github.com/osby44/TATAOnlineStore/assets/141450625/1b307412-ed3b-4989-aa90-276f4bf4c66d)

#### Question 3
![Screenshot (108)](https://github.com/osby44/TATAOnlineStore/assets/141450625/3e876fe9-c4ff-4a75-88a1-3a59ab45ec79)

#### Question 4
![Screenshot (101)](https://github.com/osby44/TATAOnlineStore/assets/141450625/aea83e52-90ad-40f2-a39c-c0604e15656d)

### Insights

•	The line chart shows a series of low sales from the beginning of the year and a steady increase from the month of August which increased massively in September, continued in the following months of October and November, but then there was a sharp decline in December. The data is incomplete for the month of December; therefore, no conclusion can be drawn from it, unfortunately. This analysis shows that the retail store sales are impacted by the seasonality which usually occurs in the last 4 months of the year.

•	All top 10 highest revenue generating countries are in Europe except Australia which is in 5th place, with Netherlands coming on top. The United Kingdom is excluded from the list as directed by Management. The UK already has high demand for the products.

•	The data shows that there is not much of a difference between the purchases made by the top 10 customers. Customer IDs 14646 & 18102 are the top 2 customers that have bought the highest revenue with 280k & 260k respectively. 12346 is on 10th position with a revenue of 77k.

•	From the map, it is evident that Western Europe and Australia are the regions that have ordered the highest volume of products.

Click [here](https://app.powerbi.com/links/6XhvrlyqdB?ctid=3922f60b-e8a2-4862-9142-e8910c694245&pbi_source=linkShare&bookmarkGuid=3ef285eb-e935-46a2-8c2d-0ca20791ce6b) to view in Power BI Service
