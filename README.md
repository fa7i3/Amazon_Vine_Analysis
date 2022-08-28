# Amazon_Vine_Analysis
# Overview
Amazon Vine program is a service that allows manufacturers and publishers to receive reviews for their products. Companies pay a small fee to Amazon and provide Amazon Vine members with programs, and in return they publish a review on the products. I analyzed the Outdoor dataset to see if there was any bias towards good reviews from Vine members. I used PySpark to perform the ETL process, transform the data, connected to an AWS RDS instance, and loaded the transformed data into pgAdmin.

# Software Used
* Google Colab
* pgAdmin
* AWS (S3 Buckets; RDS Databases)

* Dataset used:

[Amazon Review Dataset](https://s3.amazonaws.com/amazon-reviews-pds/tsv/index.txt)
# Results
I used Amazon Web Services (AWS) to retrieve the data into our Postgres Database.

* How many Vine reviews and non-Vine reviews were there?

According to the dataframe below, there are 107 Vine reviews (total_paid_reviews) and 39,869 non-Vine reviews (total_unpaid_reviews).

![question 1a](https://user-images.githubusercontent.com/104453593/187064742-1b0d1eda-7c59-4d82-9015-044d6753cae5.PNG)


* How many Vine reviews were 5 stars? How many non-Vine reviews were 5 stars?

According to the dataframe below, there are 56 Vine reviews with 5 stars (five_star_paid_reviews) and 21,005 non-Vine reviews with 5 stars (five_star_unpaid_reviews).

![question 2a](https://user-images.githubusercontent.com/104453593/187064833-ebaa26d2-919e-4ac8-87b9-f03535a3c2ed.PNG)


* What percentage of Vine reviews were 5 stars? What percentage of non-Vine reviews were 5 stars?

According to the dataframe below, the percentage of Vine reviews with 5 stars (five_star_paid_percentage) was 52.336448598130836 and the percentage of non-Vine reviews with 5 stars (five_star_unpaid_percentage) was  52.68504351751988.

![question 3a](https://user-images.githubusercontent.com/104453593/187064944-c66df4b2-9fb4-4505-bdcb-eb822c8a8c2a.PNG)

# Summary
According to the percentages of 5-star reviews for both Vine and non-Vine members, it is safe to say that there is no positivity bias towards favourable reviews in the vine program. The calculated results show that the 5-star reviews from Vine members was 52.336448598130836% (52.34%) and the 5-star reviews from non-Vine members was 52.68504351751988 (52.69%). The 5-star reviews from non-Vine members was slightly higher than the 5-star reviews of Vine members, but not significant.

An additional analysis that can be done is to calculate the measures of central tendency (mean, meidan, and mode) of the star_rating variable. By doing this, we can see the average star ratings for both Vine and non-Vine reviewers.
