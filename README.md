# Amazon Vine Analysis


## Overview
The Amazon Vine program is a service that allows manufacturers and publishers to receive reviews for their products. Companies pay a small fee to Amazon and provide products to Amazon Vine members, who are then required to publish a review.

For this analysis, the dataset that was analyzed was for personal care reviews. I used PySpark to extract the data and run the analysis to determine if there is any bias in favorable reviews from Vine members (those who are provided products as part of the Vine program).


## Results
The dataset set chosen for analysis was reviews with greater than 20 votes and where helpful votes were 50% or more of the total votes. The results of this analysis show:
- Total reviews = 3,097
- Total reviews with 5 stars = 1706
- Percent of 5 star reviews from Vine members = .1%
- Percent of 5 start reviews from Non-Vine members = 99.9%

## Summary
In looking at the results of this analysis, it does not appear there is enough data to make an assessment. In looking at the number of reviews for Vine members, there were only 3 out of 3,097, two of these being 5 star. See screenshot below.

![Screenshot](https://user-images.githubusercontent.com/72076683/107129047-4a84f300-6888-11eb-8d4f-d9248145706e.png)

I re-ran the analysis taking into account ALL reviews, not just those with more than 20 votes and 50%+ helpful votes. The results of this are:
- Total reviews = 85,981
- Total reviews with 5 stars = 48,897
- Percent of 5 star reviews from Vine members = .0004%
- Percent of 5 start reviews from Non-Vine members = 99.9995%

In looking at both results, it appears there are not enough Vine members in this product category to determine if there is any bias for Vine reviews. The number of total Vine reviews (see screenshot below) is 32 out of 85,981 total reviews. 

![Screenshot](https://user-images.githubusercontent.com/72076683/107129375-a6e91200-688a-11eb-9238-9657f34552c9.png)

Looking at ratios of 5 star reviews, the percent of Vine member 5 star reviews (of the Vine reviews) is 75% (24/32), where the percent of non-Vine member 5 star reviews are 57%. There may be a small bias in looking at the percentages, the data is not significant.
