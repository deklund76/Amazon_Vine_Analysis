# Amazon_Vine_Analysis

## Overview
The Amazon Vine program is a service that allows manufacturers and publishers to receive reviews for their products from members paid by the program. Companies pay a small fee to Amazon and provide products to Amazon Vine members, who are then required to publish a review. The purpose of this analysis is to determine if there is any bias toward favorable reviews from Amazon Vine members when reviewing video game products. Data was pulled from the video game dataset at https://s3.amazonaws.com/amazon-reviews-pds/tsv/index.txt. The data was then filtered to contain only reviews with 20 or more votes where at least 50% of the votes rated it as helpful. It was then split between reviews written by Vine members and those by non-Vine members. Relevent statistics were then computed from the two dataframes and stored in a summary dataframe for analysis.

## Results

* ![analysis summary](https://github.com/deklund76/Amazon_Vine_Analysis/blob/main/resources/analysis_summary.png)

## Summary
As seen in the results, Vine member reviews make up just a small fraction of total video game reviews, but they do tend to be more positive as 51% of them are positive compared to just 38% for non-Vine members. For further analysis, I would suggest a two sample t-test be performed on the two datasets to determine that this is statistically significant and not just noise due to the relatively small number of Vine members.
