# Data-Cleaning-Verification-Analysis-Using-R

This is an R Markdown document for the analysis of Nathan & Dora Co’s sales data. Nathan & Dora Co is a start-up manufacturing company that produces and markets kitchen utensils in Western Nigeria. The daily sales data is stored by the sales manager in MS Excel. As a data analyst, I have been given a task to determine the validity of the sales recorded in the worksheet. 
This analysis aims to find out whether a sale is valid or not valid i.e. to determine the credibility of the sales using certain metrics/data points. The dataset has the following variables:
a.	Case id – This is a unique identifier for each record available in Dataset 1.
b.	Default_phone – This is a customer’s phone number.
c.	SN – This is a unique identifier for each product that a customer has. (a customer can have multiple products).
d.	Product – This contains the name of the product that a customer bought.
e.	Original_Sale_Date – This is the date when a customer bought the product.
f.	Validity – This column helps in identifying whether a sale is valid or not valid. 


THE BUSINESS PROBLEM:
To understand the quality of the data, I have decided to define a new metric called “Creditability”.
A sale is defined is said to be Creditable if it meets all the following conditions:
a.	The customer’s phone number is present
b.	The customer’s phone number is unique
c.	The customer’s phone number contains 12 digits
d.	The product identifier is present
e.	The product identifier is unique

Two columns need to be added to this data to show whether the sales is valid or not:
1.	Column “Creditable”, whose value is either “Creditable” if it satisfies all criteria listed above, or “Not Creditable” if otherwise 
2.	Column “Reason-for-non-creditability’ lists reasons why the sale is not creditable
