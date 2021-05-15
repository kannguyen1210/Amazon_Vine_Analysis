# Amazon_Vine_Analysis

# Overview
Using my knowledge of the cloud ETL process, I’ll create an AWS RDS database with tables in pgAdmin according to the Video Games Amazon Review dataset, and extract the dataset into a DataFrame. I'll transform the DataFrame into four separate DataFrames that match the table schema in pgAdmin. Then, I'll upload the transformed data into the appropriate tables and run queries in pgAdmin to confirm that the data has been uploaded. 

Next, I’ll use PySpark to determine if there is any bias toward favorable reviews from Vine members in my dataset. Then, I’ll write a summary of the analysis.

# Results
## Total number of reviews that was paid (through Vine) for Video Games sector:
![alt text](/images/total_paid_votes.png)

## Number of 5 star reviews that was paid (through Vine) for Video Games sector:
![alt text](/images/total_5_stars_paid_vote.png)

## The ratio of 5 stars review that was paid (through Vine) for Video Games sector:
![alt text](/images/paid_5_stars_ratio.png)


## Total number of reviews that was not paid for Video Games sector:
![alt text](/images/total_unpaid_votes.png)

## Number of 5 star reviews that was not paid for Video Games sector:
![alt text](/images/total_5_stars_unpaid_votes.png)

## NThe ratio of 5 stars review that was not paid for Video Games sector:
![alt text](/images/unpaid_5_stars_ratio.png)

# Summary
Looking at the data, we can see that for paid reviews, the number of 5 stars ratio is approximately 51% while the same ratio for unpaid reviews were only around 39%. Therefore, it is very likely that being a paid review will yield higher star rating compare to a normal ones. However, there is also significant differences regarding number of records between paid and unpaid reviews, to further strengthen our conclusion, we need to introduce more data into the paid review data set so that we are looking at 2 samples with similar sizes. Aside from raising the sample size for paid reviews, I would also conduct a Linear Regression on the ratings column to see which are the factors that contribute to a higher star rating reviews and also what is the level of significant statistically for a high star review based on the fact that it is paid or not. Of course, this can only be acomplished once we transform our Vine column data into a numeric data.