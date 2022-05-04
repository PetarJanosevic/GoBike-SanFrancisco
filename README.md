# GoBike San Francisco
## by Petar Janosevic


## Dataset

Today I'm going to analyze a dataset of a bike-sharing company which includes the duration of riding the bike, some informations about the bike user, start and end stations. The location is the San Francisco Bay area.


## Summary of Findings

Bike has 183'412 rows. How many missing values are there and in which columns?
- start_station_id -> 197
- start_station_name -> 197
- end_station_id -> 197
- end_station_name -> 197
- member_birth_year -> 8'265
- member_gender -> 8'265

After some assessment, I found out that these values are not mistakes. I will use these columns without dropping the NaN's in the visualization. 

Some people rent the bike during the entire night. After further investigations, I've found out that it doesn't change the mean since its fairly distributed on all days, hence I won't include that information. It would drop the mean in general for all days, so I don't really care since it doesn't change my conclusion at all.

Most of the customers are male and that by far. The median duration rent is about 12 minutes which makes me think that people mostly rent bikes to commute to work, school etc..

Almost every week day has twice the amount of rentals than a weekend day has. This is very important, because this strenghtens my intuition that most people who rent bikes are using them to go to work, college or whatever. 
In the bivariate part I found out that weekend days had a longer mean of duration rent than weekdays. Both informations are very important for my insights since they strengthen the commuting argument. 

I did a pie chart to find out the proportion of subscribers and customers. We have way more subscribers than customers.

First scatterplot vizualisation in the bivaratie part shows that bike users are 'young' people, which isn't really a surprise. It starts to drop at 1970 birth year. I will definitely use this and compare it later with gender and user type. There was a problem in the dataset. I assume they are wrong information and wrong information has to be deleted, because this would actually make my conclusion not 100% correct. In my opinion there were some people who are definitely too old to ride a bike, like 100+ and it wasn't a low amount. I assume data was typed in wrong. 

I created a new column age stage, seperated ages in three categorise, and this gave me great insights about the costumers. I was able to sort and visualize it by gender and user type. This visualization is great and I will use it for my conclusion. 
The mean is lower for men than for the other genders. I will keep most of the seperation charts to show insights about their customers and subscribers. The mean is lower for retired people. 





## Key Insights for Presentation

Are the people who rent bikes mostly commuters?
Yes, I'd say most people are commuters. This assumption can be made based on the hourly distribution of rentals and mean distribution of days of the week. 

What are the company's customers & subscribers gender and age?
Most people are men who rent bikes and there are more subscribers. There are a lot of older people but most of them are from the younger generation. The mean from men users are much lower than women and others. 
