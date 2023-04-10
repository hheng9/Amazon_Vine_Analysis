# Amazon_Vine_Analysis

## Overview of the analysis of the Vine program
### The task is to analyze US reviews in the automotive category written by members of the paid Amazon Vine program using PySpark libraries. Around 50 datasets are provided and the objective is to extract the data, transform it, connect to an AWS RDS instance, and load the transformed data into pgAdmin. A dataset will be chosen and transformed into four separate DataFrames that match the table schema in pgAdmin. The transformed data will be uploaded into the appropriate tables, and queries will be run in pgAdmin to confirm data upload. The analysis will determine if there is bias towards favorable reviews from Vine members, by analyzing if having a paid Vine review makes a difference in the percentage of 5-star reviews, and a summary of the analysis will be provided for stakeholders.

## Results 
### The images listed below show the total number of reviews, the number of 5-star reviews, and the percentage of 5-star reviews for the two types of paid vs unpaid reviews.

* ### The paid total number of reviews is 82.
![D2-1](https://user-images.githubusercontent.com/118647523/230822469-9857c55d-2aad-41d4-ad9b-ffe0e05f9fe2.png)

* ### The paid number of 5-star reviews is 33.
![D2-2](https://user-images.githubusercontent.com/118647523/230822498-366347b1-63d4-4d4a-a698-751702365377.png)

* ### The paid percentage of 5-star reviews is around 40.
![D2-3](https://user-images.githubusercontent.com/118647523/230822503-74e256cb-9a4e-4f4f-9b07-82966ea0a67a.png)

* ### The unpaid total number of reviews is 24,742.
![D2-4](https://user-images.githubusercontent.com/118647523/230822506-a865b887-25ac-4d88-a83c-d2d04c609cbe.png)

* ### The unpaid number of 5-star reviews is 12,807.
![D2-5](https://user-images.githubusercontent.com/118647523/230822524-dd7dce35-84cb-45d2-bf82-b13594ba407a.png)

* ### The unpaid percentage of 5-star reviews is around 52.
![D2-6](https://user-images.githubusercontent.com/118647523/230822536-7928b460-654a-455b-a4d2-8cfa89a07eef.png)

## Summary
### Based on the calculations above, the unpaid reviews have a higher percentage of 5-star ratings compared to the paid reviews. The percentage of 5-star ratings for paid reviews is 40.24%, while the percentage of 5-star ratings for unpaid reviews is 51.76%. This indicates that there may be bias in the reviews, as the unpaid reviews have a significantly higher percentage of positive ratings.

To draw any conclusions about the presence of bias, additional analysis is needed. It would be useful to investigate whether the products being reviewed are similar in both the paid and unpaid reviews. It may also be helpful to compare the language and content of the reviews to determine if there are any differences in the way paid and unpaid reviewers are describing the products.

The sample size for paid reviews is much smaller than that of unpaid reviews with only 82 paid reviews compared to 24,742 unpaid reviews. This may also impact the reliability of the results and the ability to draw accurate conclusions about bias in the reviews.
