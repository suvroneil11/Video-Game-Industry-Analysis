# Video-Game-Industry-Analysis
In this project we have performed exploratory data analysis on game sales, Twitch streaming, and esports data using R, Flourish and Datawrapper.

Please download the presentation file to access the analysis gist and the visualizations.

## Introduction
### Why this analysis?
We have all played Video games at some point of time in our life. Be it on a console like Xbox or PlayStation, or PC or a mobile phone. Many scientists have concluded that playing video games have several benefits. It can be a stress and pain reliever. For some, video games are place to socialize with other fellow gamers. 
Video games have been proven to develop problem solving skills. They help us recognize patterns better and improve our eye-coordination as well. 

We are in 2023 and it is expected that the video game industry is going to exceed $350 bn with an annual growth rate of more than 7%.  As the video game industry is growing slowly, we wanted answers for several questions that we have had about the industry. 

In this project, we have divided this analysis into 3 sections:

1. Analyzing video game sales on different platforms
2. Analyzing different metrics of video games on a streaming site (Twitch)
3. Analyzing E-Sports earnings

### About the datasets:
In this project, we will be using 3 different datasets to perform a comprehensive analysis of different aspects of the gaming industry. 

1. Video Game Sales Data(https://www.kaggle.com/datasets/holmjason2/videogamedata): This dataset includes data on video games that were published between 1980 and 2020. The dataset has 16 columns and 55,519 entries including data on the game's name, platform, publisher, genre, sales statistics broken down by area, and user reviews.
   This dataset can be used to investigate the relationship between user ratings and sales figures, identify popular genres and platforms, and analyze trends in the video game industry.

2. Top Games on Twitch 2016 - 2021(https://www.kaggle.com/datasets/rankirsh/evolution-of-top-games-on-twitch): In this link, there are two datasets (csv files). First one has data about top 200 games based on number of hours watched on Twitch from 2016-2023 and second one has overall information about Twitch over the years like total watch hours month wise and year wise.
   The title of the dataset is misleading as it says from 2016-2021, but in the dataset, it also has data for 2022 and January 2023. 

3. Esports Earnings 1998 - 2023(https://www.kaggle.com/datasets/rankirsh/esports-earnings): The eSports Earnings dataset available on Kaggle provides information about the earnings of professional players and teams in the field of eSports. The data has been collected from various sources, including tournament organizers, team managers, and individual players.
   The data covers earnings from 1998 to 2023, and it is regularly updated with new information. This dataset can be useful for data analysts, researchers, and gamers who are interested in the eSports industry, its growth, and the distribution of earnings among players and teams.

## Overview of Gaming Industry
- #### Visualizing the Growth and Dominance of Publishers in the Gaming Industry
  The race chart visualizes number of games released by publishers from 1977 to 2020, it is worth noting that the gaming industry has experienced remarkable growth and evolution since its inception.
  The data clearly demonstrates this trend, showing a consistent increase in the number of games published each year.

  One of the most notable findings from the data is the dominance of Activision in the gaming industry, with a staggering 1024 games published from 1977 to 2020. This can be attributed to the fact that Activision has been a major player in the industry since the early days,
  and has consistently released popular and critically acclaimed games across a wide range of genres and platforms.

  Following closely behind Activision is Ubisoft, which has published 950 games over the same period. Ubisoft is known for its wide range of game titles across various genres, including popular franchises like Assassin's Creed, Far Cry, and Tom Clancy's Rainbow Six.

  Electronic Arts (EA) is another major player in the gaming industry, with 829 games published between 1960 and 2020. EA is best known for its sports games, such as FIFA, Madden NFL, and NBA Live, but has also published a wide range of other popular titles, including The Sims and Battlefield

- #### An Overview of Publishers and Platforms in the Gaming Industry
  The chart provides a comprehensive view of the gaming industry by including data on a wide range of publishers and platforms. It includes popular publishers like Electronic Arts and Activision, who are well known for releasing popular games such as the Call of Duty and FIFA series, along with lesser-known publishers like Idea Factory and Majesco. 

   -   The data highlights the dominance of a few popular gaming platforms, with PlayStation 2 (1170 games), PlayStation 3 (648 games), and Xbox 360 (470 games) accounting for the majority of game releases.

   -   Interestingly, Nintendo, a major player in the gaming industry, has released games on several platforms such as 3DS, DS, GBA, and Wii but lags behind in terms of the number of games released compared to other leading publishers. This could be due to a variety of factors such as a more selective release schedule or a focus on developing games that appeal to a specific audience.

   -   This data is essential in understanding the dynamics of the gaming industry and the distribution of game releases across different publishers and platforms. It is evident that some publishers and platforms dominate the industry, while others struggle to compete.

- #### Top Games sold across all platforms
  The Rshiny plot displays top games based on the total number of copies sold in millions. Each bar on the graph represents a game, with the length of the bar representing the total number of copies sold for that game.

   -   The game with the highest rank is Wii Sports, which has sold 82.9 million copies due to its inclusion with the popular Nintendo Wii console and its simple, intuitive gameplay that appeals to players of all ages and skill levels.

   -   Following Wii Sports is Super Mario Bros., which has sold 40.24 million copies and maintains its popularity thanks to its iconic characters, colorful worlds, and addictive gameplay. 

   -   Finally, Counter-Strike: Global Offensive takes the third spot with 40 million copies sold, due to its dedicated fan base, competitive gameplay, and frequent updates.

   Overall, the success of these games can be attributed to various factors such as innovative gameplay, strong branding, broad accessibility, and a loyal fan base.

- #### Analyzing User Scores and Critics Scores of Top Video Games
  Based on the chart, we can infer that:

   -   The highest-rated game among critics is Super Mario Bros. with a perfect score of 10, followed closely by Minecraft with another perfect score of 10 and the highest-rated game among users is Mario Kart Wii with a score of 9.1, followed by New Super Mario Bros. Wii with a score of 9.2.

   -   PLAYERUNKNOWN'S BATTLEGROUNDS received a significantly lower user score compared to its critic score, suggesting that it may have received mixed reviews from the gaming community.

   -   Wii Sports, Wii Sports Resort, and both New Super Mario Bros. games all received high scores from both critics and users, indicating their widespread appeal.

   -   Pokemon Red/Green/Blue Version received the highest critic score of 9.4, suggesting it was highly regarded by game reviewers.
  

## Streaming on Twitch
- #### Analyzing the viewership on Twitch over the years
  Twitch has been the go-to streaming platform for people for a very long time because of it's faster monetization process and simpler ways of building a community and engaging with viewers. In the plot above, we see how the number of Twitch users has changed from 2016 to 2023. It shows how the number     of users has gradually increased from 2016 to 2019 and then increased significantly in 2020 and 2021. We believe that this might be due to COVID-19 lockdown restrictions that became the reason of people staying at home. But, in 2022, the viewership dropped for the first time after a very long time. 
  Based on our research we found that:
   
   -   Many streamers moved to other platforms like YouTube Live, Facebook Live, etc just for the sake of trying a different new platform
   
   -   Twitch banning many forms of gambling content on the platform
   
   -   Twitch made an announcement stating that it is reducing its 70/30 split of revenue for all streamers down to 50/50
   
   The average number of viewers decreased for 2023 because the dataset that we are using has only data for the month January in 2023.

- #### Comparing number of streams and viewers from 2016 - 2023
    In the plot above, we have compared the total number of streams and total number of viewers from 2016 -2023. We can clearly see that the number of streams and Viewers has been increasing since 2016 steadily. Also, the numbers have taken a big jump from 2019 to 2020. It might be that because of           lockdown restrictions, more people started streaming and more people started watching these streams while being at home.

- #### Top 5 games based on hours streamed
    This Rshiny plot shows us the top 5 games in each year from 2016 to 2023.  We can clearly see that over the years League of Legends (LoL) has been one of the top 5 games streamed on Twitch till 2021.
    After our research, we found that there might few reasons for the decline of streaming of the game League of Legends:

   -   With the launch of popular games like Overwatch 2, God of War: Ragnarok, Elden Ring, streamers have started shifting to these games in order to try something new

   -   With the League of Legends having a steep learning curve, new streamers on Twitch are choosing less competitive games or games involving stories over investing their time and energy to gain experience with LoL.
 
- #### Top games watched on Twitch from 2016 - 2023
    In the plot, we can clearly see that Lost Ark is the game with the highest number of watch hours on Twitch and among the top 5 games watched, FIFA 23 had the lowest number of watch hours among the top 5. Based on our research we believe Lost Ark has a very high viewership because:

   -   During the launch of the game, there were several issues with the game which gained the interests of large number of gamers

   -   It's a free-to-play game, so anyone can download and play it. Now because of this, more number of viewers might become interested in watching the game streams in order to upskill their in-game skillset

   -   In 2022, it also won the Player's choice ARPG of the year award which might have spiked the interest level for viewers

   After conducting a brief research, we found that there might be few reasons why FIFA 23 had the lowest hours watched among the top 5 games:

   -   The game launched in last quarter of 2022, compared to games like Lost Ark which came out in 2019. In a short span of less than 6 months, the game has already reached such high watch hours

   -   FIFA over the years has often been criticized for it's bad servers because of which players face lot of input lag while playing online. In FIFA 23, as they introduced cross-platform gameplay, this problem has sky-rocketed which may have become the reason of players and viewers losing interest in        this game
