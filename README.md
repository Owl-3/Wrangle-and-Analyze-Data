
0.2.1 Assessing Report:

I extensively assessed the data and used the primary parameters to determine data quality:
0.2.2 Quality issues
Data quality is determined by the following parameters:
• Completeness: availability of missing data
• Validity : Different columns have right data input
• Accuracy : columns have right data types. No duplicates.
• Consistency
1. dog names: some dogs have ’None’ as a name, or ’a’, or ’an.’
1
2. A lot of missing data in, retweeted_status_timestamp, retweeted_status_id,
retweeted_status_user_id
3. timestamp is an object
4. p1, p2, p3 are column duplicates of image dataframe
5. retweeted_status_timestamp is also an object instead of datetime
6. rating_numerator goes up to 1776
7. rating_denominator should be a standard 10, but there are many values above 10
8. the source column still has the HTML tags

0.2.3 Tidiness issues:
On tidy issues, I was able to identify the following:
1. The last 4 variables of twitter_archive are relatable therefore can form one column
2. p1, p2, p3 seems relatable therefore can be combined to form one column

0.2.4 Cleaning Report:
0.2.5 Issues:
I defined the following issues in my data cleaning process:
• Merge the clean versions of twitter_archive, image_df, and tweet_df dataframes. • Create
one column for the various dog types: doggo, floofer, pupper, puppo then drop other
unnecesary columns
• Converting rating_numerator and rating_denominator into float
• Remove unnecessary columns for easier manipulation
• Change the timestamp to correct datetime format from object
• Creating a rating column
• creating month column
• remove missing values


Key Insights From Visualizations
 The following are the key insights I came up with after visualization and analysis:
 1. Floffer has the highest rating while pupper has the least rating
 2. Floofer and puppo have almost similar amount of likes while pupper has the least
 3. Floofer has the highest number of retweets while pupper has the least
 4. Pupper is the most popular dog breed while floofer is the least one
 