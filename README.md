# Business-Analytics-Predicting-Catalog-Demand
Using multiple linear regression model to predict customer demand in order to make business decision

This project was completed to practice multiple linear regression model and making business decisions. The original data and project was created by Udacity, from the Nanodegree 'Predictive Analytics for Business Nanodegree'. The original project used Alteryx to build the model, which is way easier than using Python. For practice purposes, I used Python to build the model and calculated the result which is similar to the right answer.

## Project Overview (Provided by Udacity)
### The Business Problem
You recently started working for a company that manufactures and sells high-end home goods. Last year the company sent out its first print catalog, and is preparing to send out this year's catalog in the coming months. The company has 250 new customers from their mailing list that they want to send the catalog to. 

Your manager has been asked to determine how much profit the company can expect from sending a catalog to these customers. You, the business analyst, are assigned to help your manager run the numbers. While fairly knowledgeable about data analysis, your manager is not very familiar with predictive models.

You've been asked to predict the expected profit from these 250 new customers. Management does not want to send the catalog out to these new customers unless the expected profit contribution exceeds $10,000.

### Details
1. The costs of printing and distributing is $6.50 per catalog.
2. The average gross margin (price - cost) on all products sold through the catalog is 50%.
3. Make sure to multiply your revenue by the gross margin first before you subtract out the $^.50 cost when calculating your profit.

### Data
p1-customers.xlsx: This dataset includes the following information on about 2300 customers.

p1-mailinglist.xlsx: This dataset is the 250 customers that you need to predict sales. This is the list of customers that the company would send a catalog to.

Score_No: The probability that the customer will not respond to the catalog and not make a purchase.

Score_Yes: The probability that the customer will respond to the catalog and make a purchase.

## Language used
Python

## Packages used
pandas, matplotlib.pyplot, numpy, seaborn, sklearn, statsmodels

## Files in this project
p1-customers.xlsx: The dataset includes information on about 2300 customers.

p1-mailinglist.xlsx: The dataset with information on 250 new customers.

Predicting Catalog Demand Code.ipynb: The Python code I wrote and the result of this project.

## Concept used in this project
Cross industry standard process for data mining (CRISP-DM), Predictive methodology map, Linear regression, R squared.

## Analysis before running the model
### What decisions need to be made?
We need to determine how much profit we expect if we send out the catalog. If the profit is more than $10000, then we will send out the catalog.

### What data is needed to inform those decisions?
First, we need to run a corrlation test on past information to figure out what variables is related to the sales, then we can use those variables to run a linear regression model. With the model, we can predict the sales for the 250 new customers. With the predicted sales amount, we calculat profit by multiplying predicted sales and the probability that they will make a purchase, which is the Score_Yes. After that, we calculate profit margin and subtract printing cost to get the total profit prediction.

## Conclusion after running the model
The predicted total profit is $21851, which is higher than 10000. We will send out the catalog to the 250 new customers.

## Others:
If this project inspired you, gave you ideas to help with your own project, please consider [buying me a coffee](https://www.buymeacoffee.com/emmaxsui8).
