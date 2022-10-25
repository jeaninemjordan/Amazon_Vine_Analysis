# Amazon_Vine_Analysis
 
## ETL and meta-analysis of Amazon Vine reviews with AWS, PostgreSQL, PySpark and Google Collab Notebook. 

PIC

““Learning to choose is hard. Learning to choose well is harder. And learning to choose well in a world of unlimited possibilities is harder still, perhaps too hard.”
― Barry Schwartz, The Paradox of Choice: Why More Is Less

### Project Overview

Customer feedback does not just benefit the shoppers looking for the perfect product. It is also one of the most impactful ways to help increase a business’s conversion rates, online presence, and boost a brand’s reputation. In a world where there are seemingly endless choices a finger click away, good or bad customer ratings can make or break purchases and persuade shopping decisions on consumer levels, as well as improve business practices when analyzed.

Amazon has more than two hundred million monthly visitors in the U.S., accounting for more than 37% of all online retail sales in the U.S. and accounting for over $385 billion dollars in net sales yearly. As the company continues to grow rapidly, customers increasingly make their purchase decisions with assistance from Amazon customer reviews. 

The purpose of this project was to conduct a meta-analysis of Amazon reviews and analyze the reviews as part of the Amazon Vine program, where select members of Amazon’s reviewing community are compensated to review sample products. In this analysis, the possibility of bias towards favorable reviews from the paid Vine members in the available data is analyzed. 

Fifty data sets for different product categories from 2015 were offered to choose from for this project. In this analysis, the children’s’ toys category was selected. The initial cleaning and transforming of the data set was conducted using AWS, PostgreSQL, pgAdmin, and PySpark in Google Collab. The data analysis segment was conducted using PySpark and Google Collab.

### Resources

#### Data

* s3.amazonaws.com/amazon-reviews-pds/tsv/amazon_reviews_us_Toys_v1_00.tsv.g

#### Software

* Amazon Web Services: RDS, S3
* Google Collab
* pgAdmin 6.8
* PostgreSQL 13.7
* PySpark 3.2.2
* Python 3.7.6

### ETL Process


### Amazon Vine Analysis

The data was filtered to show those that had more than twenty votes and were over 50% helpful. Calculations were conducted using the filtered data sets to produce the following results:

* Out of a total of 63,270 reviews in the entire dataset, 62,004 reviews (97.9%) were unpaid, and 1,266 reviews were paid (2.0%).

PIC

* Out of a total of 30,397 five-star reviews, 29,965 (98.5%) were unpaid, while only 432 (1.4%) were submitted by paid reviewers.

PIC

* Five star paid reviews as percent of total paid reviews – 34.12%. 

PIC 

* Paid reviews as percent of total five star reviews -  1.42%

PIC 

* Five star unpaid reviews as percent of total unpaid reviews – 48.32%

PIC

* Five star unpaid reviews as percent of total five star reviews – 98.58%

### Conclusion

Most of the reviews analyzed were submitted by unpaid participants, making up 98.5% percent of the data reviewed. Paid reviews only made up for 1.42% of the total five-star reviews analyzed, while paid five-star reviews made up for 34.12% of the 1.42% paid reviews analyzed. 

The final analysis infers that there is not a strong bias towards five-star reviews from the paid Amazon Vine reviewers versus from the unpaid Amazon reviewers. Amazon Vine reviewers are assumingly more critical submitting their reviews, as seen by the low percentage (34.12%) of five-star reviews analyzed in this project. 

To further this analysis, it would be beneficial to study the statistical distribution (mean, median and mode) of the star ratings from the paid Vine reviewers and unpaid reviewers using the full data set as well as the filtered data set.
