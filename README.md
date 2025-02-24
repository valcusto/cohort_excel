# Cohort Analysis

## Business problem

SuperStore is a supermarket chain with multiple physical stores that aim to supply various consumer products. Recently, the management team at SuperStore identified a challenge: customer retention. They observed that despite the sales growing, the frequency of recurrent customers buying at the store has decreased. Due to that, the new analysis is to understand why the customers stop buying at SuperStore and offer a solution to retain the customer.
This project aims to answer 3 main questions:
1.	What is causing customers to stop buying at the SuperStore?
2.	What initiatives can reverse this behaviour?
3.	How can SuperStore increase its customer loyalty? 

## Solution

To address this problem, I will use the cohort analysis. To plan the solution, I will follow the five key steps of data analysis:
1.	Define the fact: This critical step helps to 1) establish the aim of the analysis, 2) identify relevant business events, and 3) select the appropriate metrics for the analysis.
2.	Define the dimensions: Dimensions are qualitative attributes that provide context to the fact.
3.	Combine fact and dimensions: this step characterizes the fact by linking it to the dimensions, providing meaningful context and insights. 
4.	Select appropriate visualization tools: choosing the right graphical tools ensures the data is presented clearly and effectively. 
5.	Present macro and micro views: the final step involves providing macro perspectives (broad trends) and micro-level details (specific insights) of the fact. 
The solution's planning involved applying the SAPE method developed by the Comunidade DS. This method encompasses the definition of an output (SA: saida), the process (P), and the input (E: entrada).

## Planning (SAPE and Five steps of data analysis)**
1.	Define the fact
Customer ID
2.	Define the dimensions
Column	Dimensions	Description
Order Date	Time	When?
Ship Date		
Ship Mode	Delivery	How?
Customer ID	Customer	Who?
Sales	Product	What?
Quantity		
Discount		
Product ID		
3.	Combine fact and dimensions
1.	Customer number (fact) who placed a new order (Order Date) in the months following their first purchase (Order Date).
4.	Hypothesis
Which panels will answer the question? A retention cohort table
	
5.	Select appropriate visualization tools.
Graph	Message	Vizualization
Customer number who placed a new order in the months following their first purchase	1.	Retention	1.	Table
6.	Output (Saida)
A table with the customer ID, acquisition month, activity month and elapsed month.

7.	Process (CRISP-DS method)
a)	Combine tables
b)	Define cohorts
c)	Find the customer acquisition month
d)	Define the time (in months) from the active purchase until the first purchase (Activity month)
e)	Built the Cohort table
f)	Result interpretation

8.	Input (Entrada)
Orders.csv file – Acquisition month | Active month | Month passed
Customer.csv file – Customer ID

## Results and insights

We analysed the supermarket's cohort from January 2014 to November 2017 to measure and understand customer retention. In total, we identified 47 months from 2014 to 2017. However, we focus on the cohorts of 2014. We found that the cohorts of 2014 have a maturation of 36 months. On the month 36, the cohorts of November and December presents the highest value. In another word, the customer that first acquired a product from the supermarket in November and December, after 36 months, 31% of the customers returned (Figure 1). 
  
Figure 1: Cohort table of 2014. 

Interestingly, we also found that every 12 months that is a decrease in the customers retention. This is a trend that required further investigation in order to improve the retention every 12 months.
