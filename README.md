# Amazon-Vine-Analysis

## Project Overview
In this assignment, we assist SellBy with a project to analyze Amazon reviews by participants of the Amazon Vine program. Our goal is to analyze the dataset and determine if there is any positivity bias by Vine members versus non-Vine members by comparing total reviews and 5-star ratings.



### Data Source:
- [US Video Games - Amazon Reviews](https://s3.amazonaws.com/amazon-reviews-pds/tsv/amazon_reviews_us_Video_Games_v1_00.tsv.gz)
 
### Software / Services:
- AWS
- PostgresSQL database
- pgAdmin
- Google Colab

<br>

Our initial dataframe after importing the dataset:


![Amazon Vine Analysis - US Video Game Reviews](./images/us_video_games_reviews.png)


## Reviews
<br>

In total, there were 1,785,997 total reviews for U.S. video game reviews.

Targeting the more helpful reviews (at least 20 votes), we end up with 40,565

As for 5-star reviews, there were a total of 1,026,924 five star reviews

![Amazon Vine Analysis - Total Reviews](./images/total_reviews.png)

<hr>
<br>

Focusing on paid (Vine) reviews, we counted 94 in total, 48 of which had 5-star ratings. 51% of all paid reviews indicated a 5-star rating.

![Amazon Vine Analysis - Total Paid Reviews](./images/total_paid_reviews.png)

<hr>
<br>

Lastly, 40,471 reviews were unpaid (non-Vine). 15,663 of which consisted of a 5-star rating, leading to roughly 39% of all unpaid reviews providing a 5-star rating.

![Amazon Vine Analysis - Total Unpaid Reviews](./images/total_unpaid_reviews.png)

## Summary

Although Vine reviews were severely limited compared to non-Vine reviews (94 vs 40,471), Vine reviews had a higher percentage of being 5-star. This does show positivity bias for reviews in the Vine program as significantly less non-Vine reviews consisted of 5-star ratings.

This can mean that since Vine participants are required to review products, many may feel inclinded to provide a positive rating versus those who receive no incentive for reviewing a product, providing a more honest opinion.

Since there's a large gap between Vine and non-Vine reviews, further analysis can focus on the summary statistics for each breakdown to identify and consider the spread of data. Visualizations such as bar charts and scatter plots can assist in this analysis.
