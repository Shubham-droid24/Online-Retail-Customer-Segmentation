# Online Retail Customer Segmentation
AlmaBetter Verified Project

![image](https://github.com/Shubham-droid24/Online-Customer-Segmentation/assets/72461022/135e985d-d5bc-44a8-8a5f-4b2cfb97faa3)

I have built machine learning models to solve the unsupervised clustering problem to identify major customer segments for an online retail company. I have used K-Means and Heirarchial Clustering algorithms to solve the problem and got the best results with K-Means Algorithm.

## Problem Statement: 

In this project,  task is to identify major customer segments on a transactional data set which contains all the transactions occurring between 01/12/2010 and 09/12/2011 for a UK-based and registered non-store online retail.The company mainly sells unique all-occasion gifts. Many customers of the company are wholesalers.

## Why do we need to do this project?

The goal of customer segmentation is to help you tailor your marketing techniques to meet the specific needs of each customer group and through this form of marketing, you get to interact with your customers more effectively.

Customer segmentation allows you to identify the needs of each segment easily. As a result, it becomes easier to point out groups that need extra attention, those with the highest potential value, those with a high churn rate, etc.

This knowledge helps fine-tune and optimize offerings and products or services to meet your consumers needs and expectations. Such offerings include promotional and sales offers tailored towards specific customer segments.

As a result, businesses can then get a better understanding of things customers could be interested in. This promotes the expansion of new products and services relevant to their target audiences.

This project involves solving a real-world retail problem to identify major customer segments on a transactional dataset by building machine learning algorithms.

## Summary:

I have summarized the project in 4 steps that how the flow of the project goes:-

First, I understood the Online retail dataset in which we are provided with all the transactions occurring between 01/12/2010 and 09/12/2011 for a UK-based and registered non-store online retail.The company mainly sells unique all-occasion gifts. Dataset has 541909 rows and 8 columns and there are some duplicate rows which are 5268. It has missing values in 2 columns - Description and Customer ID. I understood all the variables and how they can be important in cluster segmentation.

Second, Dropping the duplicate rows, Dropping Invoice Numbers which starts with 'C' as it indicates a cancellation and dropping the rows having Quantity and Unit Price as negative because they should be positive values. Creating new features - Year, Month, Day and Hour from the Invoice Date column in order to use them for visualization purpose.

In visualization, I started from univariate analysis to bivariate and multivariate analysis in order to understand the relation and impact or importance of the variables. From the visualization, I defined and tested three hypothesis and fail to reject 2 of them and reject the other based on the p-value more or less than the signiicance level(0.05).

Third, I have done preprocessing which is important before model implementation. In this, I handled missing values and treated outliers , some feature engineering selection done to create new features and remove old ones.

After having selection of important features I transformed some of them and feature scaling. All these were important to be done as they create a great impact on the model performance.

Last, I build different models to cluster the customers on the basis of Recency, Frequency and Monetary value and found the best model as K-Means with k = 2 based on the silhouette score.

## Conclusion:

Some important conclusions drawn from the project are as follows:

From Visualization:

1) Most number of customers are from United Kingdom.

2) The Product name that is most bought is White Hanging Heart T-Light Holder

3) The Months in which most number of customers has bought are November, December, October and September.

4) The Days in which most number of customers has bought are Thursday and Tuesday.

5) The Peak Hours in which customers has bought the most are around 12 PM to 3 PM.

From Hypothesis Testing :

1) Average sales of customers from United Kingdom is less than or equal to average sales of customers from Germany. ( Most number of customers are from United Kingdom and Germany )

2) Average sales in the month of November is less than or equal to average sales in the month of February . ( Most number of customers purchased on November and least of them purchased on February )

3) Average sales on Thursday is not less than or equal to average sales on Sunday . ( Most number of customers purchased on Thursday and least of them purchased on Sunday )

From Model Implementation :

K-Means Clustering Algorithm using hyperparameters(k-value, init, n_init and max_iter) gave the best results to cluster the customers on the basis of Recency, Frequency and Monetary value. K-Means with K=2 has the silhouette score of 0.40 which means data points are quite well clustered and it is chosen as the final model for prediction.
