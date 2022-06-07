# dog-ratings-analysis
I reveal some interesting insights into dog ratings by Twitter user @dog_rates

# Project Background
Twitter user @dog_rates is a popular twitter user that rates pictures of dogs and awards a score based on their unique rating system. The rating goes from 7 to 15 out of 10. dog_rates gave their tweets archive to Udacity. My goal here is to derive some insights into the ratings and reveal some key insights into their past ratings. 

## Insights from my analysis:

1. Top 10 Highest rated dog breeds on average: For this insight, I only considered dog breeds with at least 20 ratings, Then I found the average of those ratings. I used a vertical bar chart to visualize the result obtained
![](https://github.com/abdulj007/dog-ratings-analysis/blob/main/Highest%20rated%20dog%20breeds.png)
 
 From the insights above, we see that the Samoyed is the highest rated dog breed on average with a score of 11.73/10. However, the difference between their rating in the top 10 is quite close. With a 0.63 difference between the 1st and 10th highest rated dog breed. Below is a table with the precise rating and rating count of the top 10 highest-rated dogs
 
 |Dog breed       | Average rating | Rating count|
 |----------------|----------------|-------------|
 |Samoyed          | 11.73          | 42         |
|Golden_retriever | 11.64          | 149         |
|Chow              | 11.64          | 44         |      
|Pembroke          | 11.44          | 88         |
|Cocker_spaniel    | 11.40          | 30         |
|Siberian_husky    | 11.30          |20          |
|French_bulldog    | 11.24          |25          |
|Pomeranian        | 11.13          |37          |
|Labrador_retriever| 11.11          | 96         |
|Toy_poodle        |11.10           |38          |


2. Most popular dog sizes - For this insight, I summed up the retweet count and favorite count for each tweet in a column called ‘engagement_score’. Then I found the sum of the engagement score for each breed and sorted it in descending order. Below is a table of the dog size with the highest engagement score.

|Dog stage        | Engagement score | 
|-----------------|------------------|
|pupper           |1,683,634         |
|doggo|1,523,702|
|puppo| 553,944|
|doggo,pupper| 158,329|
|doggo, puppo| 58,248|
|doggo, floofer| 17,695|

From our tweet archive, The pupper dog size has the most engagement with 1,683,634 engagement score. While the doggo, floofer combination is the least engaged dog stage with a 17,695 engagement score

3. Top 10 most popular dog breeds - Similar to the highest rated dogs on average insight, I found the most popular dog breeds. Popularity in this context is the most tweeted dog breed from the tweet archive
![](https://github.com/abdulj007/dog-ratings-analysis/blob/main/top%20dog%20breeds.png)

From the visualization above, we see that the golden and labrador retriever are the most tweeted dogs. Perhaps it's because retrievers are the most popular dog breeds for dog owners.

4. Does higher ratings correlate with higher favorite and retweet count? -  To test this hypothesis, We'd plot a scatterplot and correlation matrix of the ‘combined_score’ column and the ‘ratings_numerator’ column to determine this relationship

![](https://github.com/abdulj007/dog-ratings-analysis/blob/main/not%20related.png)

![](https://github.com/abdulj007/dog-ratings-analysis/blob/main/correlation%20matrix.png)

With a correlation score of 0.022 and the unclear direction of the scatterplot, I can
conclude that higher ratings do not correlate with a higher retweet and favorite count
