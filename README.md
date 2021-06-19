# Amazon_Vine_Analysis

## Overview
The purpose of this project was to analyze Amazon reviews the were curated by members of the Amazon Vine program, and determine whether there is any bias towards favourable reviews from the paid Vine members. For this analysis, I used dataset containing reviews on toys. I then leverages PySpark to create an ETL process and connected it to an AWS RDS instance where the transformed data was finally loaded into pgAdmin. From there I leveraged Pandas in Python to decipher any biases present in the data set. 

## Results
### How many Vine reviews and non-Vine reviews were there?
- Total number of Vine reviews: 1,266 reviews
- 
![tot_paid_reviews.png](https://github.com/vanessamignelli/Amazon_Vine_Analysis/blob/main/resources/tot_paid_reviews.png)

- Total number of non-Vine reviews: 62,028 reviews
- 
![tot_unpaid_reviews.png](https://github.com/vanessamignelli/Amazon_Vine_Analysis/blob/main/resources/tot_unpaid_reviews.png)

### How many Vine reviews were 5 stars? How many non-Vine reviews were 5 stars?
- Total five-star Vine reviews: 432 reviews
- 
![tot_paid_5star.png](https://github.com/vanessamignelli/Amazon_Vine_Analysis/blob/main/resources/tot_paid_5star.png)

- Total five-star non-Vine reviews: 29,982 reviews
- 
![tot_unpaid_5star.png](https://github.com/vanessamignelli/Amazon_Vine_Analysis/blob/main/resources/tot_unpaid_5star.png)

### What percentage of Vine reviews were 5 stars? What percentage of non-Vine reviews were 5 stars?
- Percentage of five-star Vine reviews: 34.12%
- Percentage of five-star non-Vine reviews: 48.34%

## Summary
Based on the analysis conducted it can be concluded that there was no bias towards reviews written by Amazon Vine program members. As displayed in the analysis above only 34% of all paid Vine reviews were 5-stars, while 48% of all non-paid reviews were 5-stars. An additional analysis that could be completed to further confirm there is no bias would be to look at the percentage of 5-star votes amoung the reviews that were not voted as helpful. Through this we would be able to determine if the volume of 5-star votes will increase across paid Vine users, but they are just not perceived as helpful.
