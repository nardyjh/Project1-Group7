# Project1-Group7: Steam & IMDB Game Data Insights

## Project Summary

The gaming industry has rapidly grown in size over the past decade, driven by exponential technological advances and boosted by the pandemic lockdowns. According to a report from PwC cited by the World Economic Forum[1], global gaming industry revenues are expected to exceed $320 billion by 2026. With a high number of competitors and an increasing variety of gaming options (both offline and online, on different platforms), studios require reliable information and data upon which to base their future plans and strategic decisions.

The goal of this project is to provide concrete data and analysis to assist game studios in making informed decisions and effectively navigating the dynamic gaming landscape. The project involves analyzing video game datasets from Steam and IMDB and visualizing various aspects.

## Table of Contents
- [Data Exploration](#data-exploration)
  - [Platforms and Marketing Analysis](#platforms-and-marketing-analysis)
  - [Category and Trends Analysis](#category-and-trends-analysis)
- [Data Sets](#data-sets)
- [Dependencies](#dependencies)
- [How to Run](#how-to-run)
- [Future Work](#future-work)
- [Acknowledgments](#acknowledgments)
- [License](#license)
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

## Data Sets

- [IMDB Video Games Dataset](https://www.kaggle.com/datasets/muhammadadiltalay/imdb-video-games)
- [Steam Game Data](https://data.world/craigkelly/steam-game-data)

[1] [World Economic Forum - Gaming Industry Growth](https://www.weforum.org/agenda/2022/07/gaming-pandemic-lockdowns-pwc-growth/)

## Dependencies

This project uses Python libraries such as Pandas, and Matplotlib for data analysis and visualization. You can install these libraries using pip:

```bash
pip install pandas matplotlib
```

## How to Run
If you wish to run the analysis scripts in this project, follow these steps:

Clone this repository to your local machine.
Install the required dependencies (as mentioned in the "Dependencies" section).
Run the Python scripts provided in the project directory to reproduce the analysis.

## Future Work
In the future, we plan to expand this project by:

Conducting more in-depth analyses on specific aspects of the gaming industry.
Incorporating additional datasets to gain a more comprehensive understanding of the market.
Developing predictive models to forecast gaming trends and success factors.

## Acknowledgments
We would like to acknowledge the contributors of the IMDB Video Games Dataset and Steam Game Data for providing valuable data for this analysis.

## License
This project is licensed under the MIT License. 

## Authors
Jorge Nardy

Kamal Farran

Muhammad Kashif 

Jude Silva

## References
World Economic Forum - Gaming Industry Growth
