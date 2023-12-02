# Customer Churn Analysis

## Introduction
Customer churn, also known as customer attrition or customer turnover, refers to the phenomenon where customers cease their relationship with a business or service provider. It is a crucial metric for companies across various industries as retaining existing customers is generally more cost-effective than acquiring new ones.

## Problem Statement
Our organization is struggling with customer churn due to the absence of real-time visibility into customer behavior and engagement.
Without timely insights, our retention efforts are reactive rather than proactive. 
As a data analst you are to develop a comprehensive dashboard that provides real-time analytics on customer interactions, enabling the team to identify potential churn risks promptly and implement targeted retention strategies.

## Tools
Microsoft Power BI was used to clean  and transform the data and also used to build the dashboard

## Data Source
The dataset used for this project can be download [here](https://drive.google.com/file/d/17bUJhEkQEDmoyLZ88TyS_Pi2IRcRMfAg/view?pli=1). 

## Meta Data
The dataset contains 10000 rows of data and 12 columns. The columns store the following data 
- Customer_id : Id of the customers
- Credit_score : 
- Country : countries of the customers
- Gender : customers gender
- Age : customers age
- Tenure : duration of customer in the organisation
- Balance : customers account balance
- Products : product purchased or used by the customers
- Credit_card : customer credit card status
- Active member : customer activity status
- Estimated salary : salary estimated that the custumer earned
- Churn : customer churn status

## Data Cleaning and Transformation
After downloading the data it was loaded into power query in Power BI for data cleansing and transformation. 
Power query is a tool used for extracting, transforming and loading data (ETL tool).

After loading the dataset null and duplicates values was checked and removed and also the data type was changed to the right format.
columns not needed for the analysis was dropped i.e (Estimated salary) column and some conditional columns was added to transform the data into useful format for analysis.
- Credit card column contains the values 1 and 0 which was replaced with "Owned" and "Not Owned". 1 was mapped to "Owned" and 0 mapped to "Not Owned"
- Active member column contains the values 1 and 0 which was replaced with "Active" and "Not Active". 1 was mapped to "Active" and 0 mapped to "Not Active"
- Churn status column contains vaues 1 and 0 which was replaced with "Churned" and "Not Churned". 1 was replaced with "Churned" and 0 replaced with "Not Churned"
- Created a new conditional column (Age_group) using the age column. The Age contain customers age which is a contionous value. 

