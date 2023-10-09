# Project1-Group7: Steam & IMDB Game Data Insights

## Project Summary

The gaming industry has rapidly grown in size over the past decade, driven by exponential technological advances and boosted by the pandemic lockdowns. According to a report from PwC cited by the World Economic Forum[1], global gaming industry revenues are expected to exceed $320 billion by 2026. With a high number of competitors and an increasing variety of gaming options (both offline and online, on different platforms), studios require reliable information and data upon which to base their future plans and strategic decisions.

The goal of this project is to provide concrete data and analysis to assist game studios in making informed decisions and effectively navigating the dynamic gaming landscape. The project involves analyzing video game datasets from Steam and IMDB and visualizing various aspects.

## Table of Contents
- [Data Exploration](#data-exploration)
  - [Platforms and Marketing Analysis](#platforms-and-marketing-analysis)
  - [Category and Trends Analysis](#category-and-trends-analysis)
  - [Games Released Month and Price Analysis](#Games-Released-Month-and-Price-Analysis)
  - [Top performer Games Analysis](#Top-performer-Games-Analysis)
- [Data Sets](#data-sets)
- [Dependencies](#dependencies)
- [How to Run](#how-to-run)
- [Future Work](#future-work)
- [Acknowledgments](#acknowledgments)
- [Authors](#authors)
- [References](#references)

## Data Exploration

### Platforms and Marketing Analysis

#### 1. Which platform has the highest player count on average?
- Explored the correlation between the number of games available on each platform and the mean player count.
- Concluded that, on average, there is no significant difference in player counts between Windows, Mac, and Linux platforms.
- Initial differences observed were influenced by outliers or limited data availability. This dataset cannot provide this information. 

#### 2. Do games with broader platform support attract more players?
- Analyzed mean rating, popularity, mean price, and PriceOwnersProduct.
- Games supporting multiple platforms tend to have higher Metacritic ratings and popularity, attracting more players and better reviews.
- Game pricing does not significantly vary based on the number of supported platforms. 

#### 3. Is there a relationship between Screenshots, Early Access Status, and Demos and the number of players?
- Analyzed scatterplots for screenshots vs. mean owners, early access vs. mean owners, and demos vs. owners.
- Weak correlation found between the number of screenshots and mean owners, suggesting other factors play a more significant role.
- Slight difference in mean owners between early access and non-early access games, but not statistically significant.
- Games with demos tend to have a higher mean number of owners, indicating a positive relationship.

#### 4. Which platform has the highest game count on average?
- Explored the correlation between the number of games available on each platform (Windows, Mac, Linux) and relevant metrics.
- Windows is the most dominant gaming platform, with a significantly higher number of games available compared to Mac and Linux.
- Games available on the Windows & Mac combination seem to have higher Metacritic ratings and recommendation counts, indicating a positive reception among users and critics.
- The combination of all three platforms (Windows, Mac, and Linux) results in the highest mean recommendation count, suggesting that cross-platform availability may lead to increased user engagement and recommendations.

### Category and Trends Analysis 

#### 5. Is there any advantage to developing a Single-Player or a multi-player game?
- Analysis of games based on whether they are single-player or multi-player games shows a significant advantage for multi-player games in terms of mean number of players, mean number of owners, mean Metacritic rating, and mean number of recommendations on Steam.
- This suggests that multi-player games tend to be more popular and successful.

#### 6. Are there any apparent genre trends across the past 3 decades?
- Analysis of the percentage of genres between 1985 and 2019 shows that while Action has been the dominant genre for decades, Adventure has been steadily rising in prominence, surpassing Action after 2015.
- Also observed is that the percentages of Family and Sci-Fi games have been decreasing, while other genres have kept relatively steady levels. It is to be noted that this does not reflect a decrease in the number of Family or Sci-Fi games, only of their percentages relative to the total number of games per year. In fact, the number of games have been increasing per year across all genres.

### Games Released Month and Price Analysis

#### 7. Find out the Month with most number of Games Released?
- From the provided data, it is found out that on steam gaming engine, 1548 games have been released in the month of "August". which could potentialy be due to some promotional season of "Back to School". 
However since we do not have any sales data. so we can not exclusively point out towards the actual reason for more numbers of games being released in the Month of August.
#### 8. Find the Games with positive increase in the intial and final price.
- while trying to find the price change from initial price to final price change, there is not a single game with positive increase from inital price to final price in past three decades of provided Data.
most games have no change in initial price and final price. Histogram shows skewed bars and mode is zero.
### Top performer Games Analysis
#### 9(a). Number of action Genre games based on Metacritic rating and Recommendation.
- more than 4000 Games in Action Genre Games did not get Meta critic Rating and Recommendation. Only one game was able to secure more than 150K Recommendation count while only 33 games 90-99 rating. Since the Top recommended and rated games have reduced in numbers. so it is good idea to follow the parameters of games in top notch for launching new game with popular in demand features.
#### 9(b). Comparison of Top 20 game based on "Metacritic Rating" and "Recommendation count" of all times and Top 20 games based on "Action Genre" for "Metacritic Rating" and "Recommendation count".
- from past three decades data, it is found that "Bioshock(tm),Half-life,Half-life2 and Grand theft Auto V" are top games based on the Metacritic Rating.
Based on Recommendation count "counter strike-Global offense,Dota 2,Fortress 2, Garrys Mod are top 4 games.
Only Grand Theft Auto V makes to Top 20 of recommendation count of all times list of provided data set.
- Action Genre based MetacriticRating and RecommendationCount Top 20 games were found and compared with all times games which indicates "Action Based Genre is rated and and recommended by players. 
From One sample t-test and Saphiro-wilk test, p_value was found. hypothesis results indicate that top-20 Games based on ratig are different for All times Top 20 games and Action Genre Based Top20 games and same applies for recommendation count based games. 
Although action genre games are played most and in high demand on steam engine but still high metacritic games do not get high recommendation count.
### Genre and popularity
#### 10. Which genres do games prefer to play the most?
-Analysis, shows that genres action, adventure and indie has beed recommended by the players most. We can also note the genres stertergy, RPG, Action, Racing and RPG have relatively high ratings from the critics
- Worst recommended genres are sports, racing and casual and the worst critic rated genres are casual, early access and free to play
- Looking at the data we can see action genre has overlap in best recomendations and crtics rating 
- Looking at the data we can see casual genre has  overlap in worst recommendation and critic rating
#### 10(b). Which genres do players choose to spend the most money ?
-Analysis shows the genres action has the most capital. This genre has the most number of owners with the highest game prices. Followed by adventure and stratergy genre. Racing genre and sports genre has the least amount of capital in it 
- Analysis shows genres with least capital are casual, sports, early access, free to play and racing 
- Also these genres of games fall in both the catergory of worst rated and recommended
#### 10(c). Which genres has the changes in demand and discounts ?
-Genres with increase in demand. If the price is increase by the platform, we can assume the genre has a higher demand. Across all the genres we can see the mean price has reduced. But we can analyse by the rate of change 
- We can see genres indie, nongame and adventure has the greatest negative mean price difference. They experience the greatest decline in demand over time and steam would most likely list these genres on discount 
- We can see genres multiplayer, action, racing and sports has the least mean price difference. They hold the demand value over time and arent as subjected to discounting 

## Data Sets

- [IMDB Video Games Dataset](https://www.kaggle.com/datasets/muhammadadiltalay/imdb-video-games)
- [Steam Game Data](https://data.world/craigkelly/steam-game-data)

[1] [World Economic Forum - Gaming Industry Growth](https://www.weforum.org/agenda/2022/07/gaming-pandemic-lockdowns-pwc-growth/)

## Dependencies

This project uses Python libraries such as Pandas, and Matplotlib for data analysis and visualization.
Numpy for price change analysis and statistics for hypothesis testing.
 You can install these libraries using pip:

```bash
pip install pandas matplotlib
pip install scipy 
pip install numpy

```

## How to Run
If you wish to run the analysis scripts in this project, follow these steps:

Clone this repository to your local machine.
Install the required dependencies (as mentioned in the "Dependencies" section).
Run the Python scripts provided in the project directory to reproduce the analysis.

## Future Work
In the future, there is potential to expand this project by:

Conducting more in-depth analyses on specific aspects of the gaming industry.
Incorporating additional datasets to gain a more comprehensive understanding of the market.
Developing predictive models to forecast gaming trends and success factors.

## Acknowledgments
We would like to acknowledge the contributors of the IMDB Video Games Dataset and Steam Game Data for providing valuable data for this analysis.

## Authors
Jorge Nardy

Kamal Farran

Muhammad Kashif 

Jude Silva

## References
World Economic Forum - Gaming Industry Growth
