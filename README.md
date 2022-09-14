# Business_Analysis
Business Analysis Made Easy

#### Video Demo:  https://youtu.be/WQIJnhX7f-c

Overview: In this project I created a program that helps users create a business model and track sales, revenue and profit over time. It consists of four key functions. The `get_business()` function has the user input business information such as name starting cash reserves, information about product lines, projected growth rates, and the amount of time they would like to track the company for. Next, he `generate_sales()` function tracks these products over time, generating random sales per day based on estimated daily sales and the projected growth rate. Finally, the program converts this to a pandas data frame and generates plots of the sales data for the time period given.

## get_business() function

#### The `get_business()` function serves as the input mechanism for the program. It prompts the user for a number of inputs including starting cash reserves, daily fixed costs, ending day (the starting day will be automatically generated as the day the program is run), and any number or product lines for the company. Each product line will consist of a product name, estimated daily sales, profit margin, and projected yearly growth rate. It will return all these values as a tuple consisting of a dictionary of the business relevant information and the ending date.

## generate_sales() function

#### The `generate_sales()` function takes the ending date and product lines given in the previous step as parameters and randomly generates daily sales for each based on +/- 10% of average sales times the projected growth rate

## create_report() function

#### The `create_report` function takes the sales data and uses matplotlib to dynamically create a pdf report for the company featuring a line chart of daily sales for each product
