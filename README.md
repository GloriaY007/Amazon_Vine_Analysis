# Amazon Vine Analysis

## Project Overview:
The main task in this project is to analyze Amazon reviews written by members of the paid Amazon Vine program and submit an analysis to the SellBy stakeholders. The analysis will determine whether or not there is any bias towards favorable reviews from Vine members in the dataset. THis will be done using PySpark to perfrom the ETL process to extract the dataset, transform the data, connect to an AWS RDS instance, and load the transformed data into pgAdmin.

The dataset of Amazon reviews I analyzed were those in the "Digital Video Games" category:
- [Amazon Reviews Dataset for Digital Video Games](https://s3.amazonaws.com/amazon-reviews-pds/tsv/amazon_reviews_us_Digital_Video_Games_v1_00.tsv.gz)
- [Large data set (from which you can find the Digital Video Games data set)](https://s3.amazonaws.com/amazon-reviews-pds/tsv/index.txt)


## Results:

|  | Total # of Reviews | # of 5-Star Reviews| % of 5-Star Reviews|
| ------------- | ------------- | ------------- | ------------- |
| Paid  | 0  | 0 | 0  |
| Unpaid  | 1685  | 631  | 37.45%  |

There were no paid reviews and 1685 unpaid reviews. Out of those, 631 upaid reviews had a 5 stars rating.

Paid Reviews:

![Paid Reviews](https://github.com/GloriaY007/Amazon_Vine_Analysis/blob/main/Screenshots/Paid%20Reviews.png)

Unpaid Reviews:

![Unpaid Reviews](https://github.com/GloriaY007/Amazon_Vine_Analysis/blob/main/Screenshots/Unpaid%20Reviews.png)

## Summary:
There does not seem to be any hint of bias in the reviews for the positivity bias for reviews in the "Digital Video Games" category Vine program. No reviews had been paid, therefore, 37.45% of the ratings are honestly given withouth any significant bias. It would seem that this is a category that has fairly small amount of review compared to what one can image, and the reviews in this category seem less bias.
