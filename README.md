# Amazon_Vine_Analysis
# Overview
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

