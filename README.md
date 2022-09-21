<<<<<<< HEAD
# 2019 Bay Wheels Ride Data Exploration
## by Odira Dancan


## Dataset

> Bay Wheels is a regional public bicycle sharing system in California's San Francisco Bay Area. It is operated by Motivate in a partnership with the Metropolitan Transportation Commission and the Bay Area Air Quality Management District. Bay Wheels is 'the first regional and large-scale bicycle sharing system deployed in California and on the West Coast of the United States. It was established as Bay Area Bike Share in August 2013. As of January 2018, the Bay Wheels system had over 2,600 bicycles in 262 stations across San Francisco, East Bay and San Jose.(info source: Wikipedia)

### Data Wrangling Process
>1. loaded necessary modules
>2. Loaded the data using pd.read_csv
>3. Used .info() and .describe() to get an overview of the dataset
>4. Handled missing values: investigated if na values are present then dropped them using .dropna()
>5. Added minutes column fron 'duration_sec' column for easier manipulation 
>6. Created a function to extract year (in string form and casted it to datetime dtype) from the data was collected to use later to calculate user age.
>7. Added age column to the dataframe using the year previously extracted by getting the difference with the 'member_birth_year' column. >8. Converted the new age column to integer.
>8. Extracted the weekday data from the 'start_time' column to use to explore weekly usage
>9. Dropped the unwanted columns for easier exploration and wrangling
>10. Filtered out outliers in 'age' column 

## Summary of Findings

>- Weekdays usually busier than weekends, maybe because people rest, attend to their religious belief, and work weekdays. Thursdays and Tuesdays usually the busiest days of the week. Summar time was the most popular season of a year, likely due to the weather.
>- On user types, there were more male riders than female, and most members were subscribers compared to non-subscribers(customers). Most users did not want to share bikes for all their trips. Most users are aged 20 to 40 years even though there are some outliers, up to 141 years olds
>- Duration taken by users were short, most lasted between 5 to 10 minutes, though there were some very long outliers like 24hrs.
>- The Other gender recorded longest duration compared to female and male while males recorded the least duration. Bike usage is higher during the week than during weekends. More males use bikes during the week than any females and other gender. Subscribers record higher bike usage across the week than customers. Thursdays and Tuesdays are the busiest days of the week. Other gender seem to have much older users that females and males. Females tends to be the youngest users. Average subscriber age is slightly higher than customer age. Other gender recorded highest duration usage compared to females and males across the week.
>- The shorter duration usage for subscribers may imply higher use for work when they're going to work suggesting they might be using the bikes mainly for work communitng. The subscribers also seems to be open to sharing, perhaps to reduce cost.

## Key Insights for Presentation

>- All Customers did not want to share bike all round the trips while subscribers heavily shared their bikes
>- Weekdays usually busier than weekends, maybe because people rest, attend to their religious belief, and work weekdays
>- There were more male riders than female, and most members were subscribers compared to non-subscribers(customers)
>- The Other gender recorded longest duration compared to female and male while males recorded the least duration
>- Subscribers record higher bike usage across the week than customers.
>- Average subscriber age is slightly higher than customer age.
>- The shorter duration usage for subscribers may imply higher use for work when they're going to work suggesting they might be using the bikes mainly for work communitng. The subscribers also seems to be open to sharing, perhaps to reduce cost.
=======
