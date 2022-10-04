# Amazon_Vine_Analysis

## Overview
Since your work with Jennifer on the SellBy project was so successful, you’ve been tasked with another, larger project: analyzing Amazon reviews written by members of the paid Amazon Vine program. The Amazon Vine program is a service that allows manufacturers and publishers to receive reviews for their products. Companies like SellBy pay a small fee to Amazon and provide products to Amazon Vine members, who are then required to publish a review.

In this project, you’ll have access to approximately 50 datasets. Each one contains reviews of a specific product, from clothing apparel to wireless products. You’ll need to pick one of these datasets and use PySpark to perform the ETL process to extract the dataset, transform the data, connect to an AWS RDS instance, and load the transformed data into pgAdmin. Next, you’ll use PySpark, Pandas, or SQL to determine if there is any bias toward favorable reviews from Vine members in your dataset. Then, you’ll write a summary of the analysis for Jennifer to submit to the SellBy stakeholders.

The purpose is uncover if there is a bias for Vine-positive reivews in the dataset

## Results: Using bulleted lists and images of DataFrames as support, address the following questions:

![Vine Review Analysis 1](https://user-images.githubusercontent.com/103234661/193838208-22d299fc-40c3-4374-a9ed-9c1e6b54ed6e.png)

![Vine Review Analysis 2](https://user-images.githubusercontent.com/103234661/193838215-4d9c7e21-7b1f-4c44-9d49-24da25d2ed79.png)


**How many Vine reviews and non-Vine reviews were there?**

There were 219 Vine reviews and 189,185 non-Vine reviews

**How many Vine reviews were 5 stars? How many non-Vine reviews were 5 stars?**

74 5 star Vine reviews were 5 stars and 98639 non-Vine reviews were 5 stars

**What percentage of Vine reviews were 5 stars? What percentage of non-Vine reviews were 5 stars?**

33.79% Vine reviews were 5 stars and 52.14% were 5 star non-Vine reviews

## Summary: In your summary, state if there is any positivity bias for reviews in the Vine program. Use the results of your analysis to support your statement. Then, provide one additional analysis that you could do with the dataset to support your statement.

There is likely not a positivity bias in the reviews for the Vine program. We determined this because of the volume of 5 star non-Vine reviews far outweighed the 5 star Vine reviews. With a 52.14% 5 star review total versus 33.79%, the non-Vine reviews from users are enjoying using the program. The sheer number of total reviews for the non-Vine reviews allow any possible outliers to be neglible. 

Additional analysis that we can provide would be to utilize the 1 star to 4 star reviews as well as finding the mean, mode, mediun and STD seperately and between the two. We can also utilize reviewsing of the program from other sources where reviews may be found and compare its statistic to those used in this dataset.
