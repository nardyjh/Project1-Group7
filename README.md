# Project1-Group7

Project Summary:

The gaming industry has been rapidly growing in size in the past decade, as technology advances exponentialy, and boosted by the pandemic lockdowns. According to a report by a PwC report quoted by the World Economic Forum[1], the global gaming industry revenues are expected to exceed $320 billion by 2026. With the high number of competitors and increasing number of ways to game (offline/online, different platforms), studios need reliable information and data on which they can base their future plans and strategic decisions. 

The goal of this project is to provide concrete data and analysis that help game studios make informed decisions and navigate the dynamic gaming landscape effectively. The project involves analyzing video game datasets from Steam and IMDB and visualizing different aspects.

Some datapoints to analyze include marketing factors (the effectiveness of game demos and how prices vary from initial release price to final price), hardware decisions (platform availability), top performing games by recommendation and Metacritic ratings (overall and by top genre), game popularity/success per different categories (single-player/multiplayer). We are also analyzing genres, including genre trends in the past 3 decades and upcoming genre trends (thorugh linear regression), and popularity/ratings by genre.


# Data Exploration
## Platforms and Marketing Analysis

## 1. Which platform has the highest player count on average?
- Calculated the average player count for each platform (Windows, Linux, Mac).
- Explored the correlation between the number of games available on each platform and the mean player count.

### Analysis
- Concluded that, on average, there is no significant difference in player counts between Windows, Mac, and Linux platforms.
- Initial differences observed were influenced by outliers or limited data availability. This dataset cannot provide this information. 

## 2. Do games with broader platform support attract more players?
- Examined the relationship between the number of supported platforms and player count.
- Analyzed mean rating, popularity, mean price, and PriceOwnersProduct.

### Analysis
- Games supporting multiple platforms tend to have higher Metacritic ratings and popularity, attracting more players and better reviews.
- Game pricing does not significantly vary based on the number of supported platforms. 

## 3. Is there a relationship between Screenshots, Early Access Status, and Demos and the number of players?
- Investigated the relationship between screenshots, demos, early access status, and the mean number of owners.
- Analyzed scatterplots for screenshots vs. mean owners, early access vs. mean owners, and demos vs. owners.

### Analysis
- Weak correlation found between the number of screenshots and mean owners, suggesting other factors play a more significant role.
- Slight difference in mean owners between early access and non-early access games, but not statistically significant.
- Games with demos tend to have a higher mean number of owners, indicating a positive relationship.

## 4. Which platform has the highest game count on average?
- Explored the correlation between the number of games available on each platform (Windows, Mac, Linux) and relevant metrics.

### Analysis
- Windows is the most dominant gaming platform, with a significantly higher number of games available compared to Mac and Linux.
- Games available on the Windows & Mac combination seem to have higher Metacritic ratings and recommendation counts, indicating a positive reception among users and critics.
- The combination of all three platforms (Windows, Mac, and Linux) results in the highest mean recommendation count, suggesting that cross-platform availability may lead to increased user engagement and recommendations.

### (5) Is there any advantage to developing a Single-Player or a multi-player game?
- Analysis of games based on whether they are single-player or multi-player games, shows a significant advantage for multi-player games in terms of mean number of players, mean number of owners, mean Metacritic rating and mean number of recommendations on Steam.
- This suggests that multi-player games tend to be more popular and successful.

### (6) Are there any apparent genre trends across the past 3 decades?

- Analysis of the percentage of genres between 1985 and 2019, shows that while action has been the dominant genre for decades, Adventue has been steadily rising in prominence, surpassing Action after 2015.
- Also observed, is that the percentages of Family and Sci-Fi games have been decreasing, while other genre have kept relatively steady levels. It is to be noted, that this does not reflect a decrease in the number of Family or Sci-Fi games, only of their percentages relative to the total number of games per year. In fact, the number of games have been increasing per year across all genres.

## Analysis Summary 
In summary, the analysis covers platform player counts, game support, the impact of screenshots, early access, and demos on player numbers, and the relationship between platform game counts and other metrics.


# DataSets

https://www.kaggle.com/datasets/muhammadadiltalay/imdb-video-games<br>
https://data.world/craigkelly/steam-game-data

[1] https://www.weforum.org/agenda/2022/07/gaming-pandemic-lockdowns-pwc-growth/
