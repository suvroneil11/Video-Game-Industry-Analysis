# Comprehensive Analysis of Video Game Industry
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
## Esports
- #### Analyzing different genres in Esports
  The plot shows the range of esports games genres, from fighting games to immersive sports simulations and everything in between. Popular Esports genres based on the plot are:
  - Fighting Game
  - First-Person Shooter
  - Sports
  - Racing
  - Strategy
 
- #### Esports through the Years
   The presented chart provides a comprehensive analysis of the esports industry's growth and trends between the years 1998 and 2023. The dataset includes data on more than 450,000 participants who engaged in more than 500 games, generating over $1 billion in
   revenue through 50,000 major and minor tournaments.
   
   The early years of esports until 2002 were characterized by a limited number of games, with only a handful offering prize money, such as Counter-Strike, Quake 2 and 3, and Starcraft. The industry was relatively small during this period, and the number of participants was limited to less than 2,000 players. Despite this, more than 200 tournaments were organized by 2002, with Counter-Strike emerging as the highest earning game,
   followed by Quake III and StarCraft. Counter-Strike had the most number of players, followed by Quake III and Starcraft. Meanwhile, Age of Empires II had the most number of tournaments organized, followed by Quake III and Starcraft.
   
   The advent of the internet and better access to technology after 2002 ushered in a new era for esports, with some key games emerging as consistent earners. Games such as Counter-Strike, Starcraft, Dota 2, and League of Legends reported consistently high earnings. On the other hand, games like Fortnite, Player Unknown Battle Grounds, Call of Duty, and various versions of FIFA and Halo showed high earnings but only for short periods of time.
   
   Some games, such as Counter-Strike, League of Legends, Call of Duty, Dota 2, Counter-Strike: Global Offensive, and Valorant, had a consistent high number of players, while others, such as Fortnite, Rainbow Six Siege, Player Unknown Battle Grounds, and Starcraft, experienced small patches of high player numbers. Additionally, consistent games such as Counter-Strike, Warcraft III, Starcraft II, League of Legends, Counter-Strike: Global Offensive, and Valorant displayed high numbers of tournaments organized for longer durations of time.
   
   Games like Super Smash Bros, Rocket League, Overwatch, and Fortnite, showed a high number of tournaments organized but in inconsistent or short durations of time. 
   
   In conclusion, the esports industry has grown significantly over the years, with key games emerging as consistent earners while others experience short-lived popularity. The industry continues to evolve, and future trends will likely depend on technology advancements and emerging gaming preferences.

- #### Total Earnings and Tournament Impact on Popular Games
  The chart presented provides valuable insights into the world of esports, highlighting the total earnings generated by various games across the number of tournaments organized. One of the key observations from the chart is the significant difference in earnings between games with similar numbers of tournaments organized. This indicates that the scale and quality of tournaments can have a significant impact on the overall earnings generated by a game.\
  The chart presented above highlights the total earnings garnered by various games across the number of esports tournaments organized. Two games that stand out prominently in the graph are Dota 2 and Starcraft II. Interestingly, despite Starcraft II having the highest number of tournaments organized, its overall earnings are comparatively low, while Dota 2, with a lower number of tournaments, has amassed over 300 million in earnings. This discrepancy can be attributed to the difference in the scale of tournaments organized for each game.

  Additionally, several other games have also demonstrated significant earnings, including Counter Strike: Global Offensive, League of Legends, and Fortnite. However, it is worth noting that Fortnite has the lowest number of tournaments organized, followed by League of Legends, with Counter Strike having the maximum number of tournaments amongst the three.

  It is noteworthy that most games fall within the earnings range of 0 to 100 million and the tournament range of 0 to 1000. These observations suggest that the esports industry is thriving, with games being able to generate significant revenue despite the relatively low number of tournaments. As the industry continues to grow, we can expect to see an increase in both the number of tournaments organized and the earnings generated by games across the board.

- #### Key Insights and Implications for Industry Success
  The chart shows the occupancy percentage of various games in the esports industry across multiple factors. By conducting an in-depth analysis of the data, we can draw several critical insights that provide a better understanding of the esports industry and the factors driving its success.

  The chart used are multiple donut charts to identify the top percentage of games for each factor, providing a consolidated view. Dota 2, despite having fewer tournaments organized compared to other games like Rocket League and Starcraft, has the highest total and online earnings and the most substantial number of players for a single game. Additionally, Fortnite has the second-highest earnings for a single game despite having fewer tournaments but with a high number of players. This observation emphasizes the vital role that tournaments play in the esports industry and suggests that investing in well-organized and high-quality tournaments may be a crucial strategy for driving success in this market.

  On the other hand, games like Counter-Strike: Global Offensive and League of Legends have equal shares in almost all of the factors. This finding indicates that the esports industry has a dynamic and ever-changing landscape where each game has unique factors contributing to its success, which can shift over time. Hence, adaptability and responsiveness are critical in the esports industry, and game developers and organizations must identify and respond to changing market conditions to maintain success.

  In conclusion, the chart provides significant insights into the esports industry. By understanding and leveraging these insights, game developers and esports organizations can position themselves better for success in this rapidly growing.

## Trends in 2016 - 2020
   In this section, we conducted a comprehensive analysis of the performance of top 5 games between the years 2016 to 2020, in terms of their total sales, watching hours on Twitch, and earnings. By comparing their rankings based on these metrics, we were able to gain valuable insights into the popularity and profitability of these games. The findings from this analysis sheds a light on the competitive landscape of the gaming industry and provide valuable information for players, developers, and investors alike.

- #### Examining the Top 5 games with the highest units sold
  The tree chart shows the top five video games in terms of total units shipped in the years they were released.

   -   With 36.6 million units shipped in 2017, PLAYERUNKNOWN'S BATTLEGROUNDS had the most overall units shipped. The game's widespread appeal can be due to its distinctive battle royale gameplay.

   -   The second-placed game in 2019 was Call of Duty: Modern Warfare, which shipped a total of 30.13 million copies. The game became a popular among players thanks to its realistic and contemporary graphics and timeless gameplay.

   -   The 2017 release Mario Kart 8 Deluxe came in third with 24.77 million units shipped. The success of the game can be traced to its ageless appeal and universal accessibility.

   -   Call of Duty: WWII, which was released in 2017, took fourth place with 19.82 million units shipped. Gamers like the game's classic World War Two backdrop and interesting storyline.

   -   Lastly, Red Dead Redemption 2, which was released in 2018, came in fifth place with 19.71 million units sold. The game's engrossing plot and massive open-world gameplay set in the Wild West won it critical acclaim and a devoted following.

   -   Overall, these top-performing titles illustrate the value of distinctive gameplay and compelling storylines in fostering success in the video game business and reflect the diverse interests of gamers around the world.

- #### Analyzing viewer hours on Twitch for top-selling games on multiple platforms
  From the previous plot, we found the top 5 games sold across all the platforms. In the above plot, we are trying to analyze trends based on number of hours spent by viewers on these games streamed on Twitch from 2016 - 2020. Based on the second dataset that we have used which contains data related to Twitch, we found that Mario Kart 8 Deluxe was only streamed in 2021 because of which it is not showing in the above plot.

   We can clearly see that PLAYERUNKNOWN'S BATTLEGROUNDS has the highest number of watch hours among the top 5 games with more than 1.4 billion hours spent by viewers. In the previous plot, we saw that PLAYERUNKNOWN'S BATTLEGROUNDS was the highest selling game overall as well. This shows that this game has been very popular among players and viewers. We believe there might be few reasons for this popularity:

   -   This game gained popularity as it was a battle royale game which could accommodate up to 100 players because of which large number of players started playing the game and watching streams in order to upskill their in game skills

   -   The game was developed using Unreal Engine 4 and the in-game mechanics gave the game a real life like feeling for the players

   -   Players could socialize with random players or play with friends with the help of text or voice chatting which made the game more enjoyable
  
   We can see that Call of Duty: Modern Warfare had the second highest number of units sold/downloaded among the top 5 games, but based on the size chart above, we can see this game was 5th based on the number of watch hours on Twitch. Also, in the second plot in the story, we see that this might be due to couple of reasons being:

   -   The game was released in 2019 while the other games were launched at least a year before, which can be the reason that the game was still on the rise and had low watch hours

   -   People were still playing other games more than this game as when this game was launched it took a lot of time for the developers to fix different bugs and issues with the game to make it more enjoyable.

   Overall, we can conclude from these two plots that even if the number of units sold/downloaded is very high for a game, that certainly doesn't mean that the game is popular on Twitch among the viewers or vice versa. We believe that even though a game might have high sales, it needs to have robust anti-cheat engine, good graphics and frequent updates from the developers so that playing experience is not hampered. Otherwise, if the playing experience is hampered for a game, people will switch to alternates for these games and it's highly likely they will start watching streams of these new games.

- #### Analysis of Top Games in Esports
  The chart shows the earnings, number of people, and tournaments for top 5 popular video games : Dota 2, Fortnite, Counter-Strike: Global Offensive, League of Legends, and Arena of Valor from 2016-2020 for Esports as the data for top 5 games isn't available/contains zero values. Here are some insights we can draw from this data:

  Dota 2 has consistently been one of the top-earning games in the past five years. Its earnings have steadily increased from 2016 to 2019 before experiencing a dip in 2020. This could be due to the pandemic and the cancellation of several tournaments.

  Fortnite has been a major player in the gaming industry since 2018, with earnings of $19.9 million that year. Its earnings peaked in 2019 at $78.5 million before experiencing a significant drop in 2020. This could be due to the game's declining popularity or the impact of the pandemic on the gaming industry.

  Counter-Strike: Global Offensive has consistently been one of the top-earning games, with earnings increasing from 2016 to 2019 before experiencing a slight decline in 2020. The game has also consistently had a high number of players and tournaments, making it a popular esports title.

  League of Legends has seen a decline in earnings since 2018, with earnings dropping from $14.7 million in 2018 to $8.7 million in 2020. However, it still remains a popular esports title with a significant number of players and tournaments.

  Arena of Valor is a relatively new game compared to the others on the list, with its first data point in 2016. Its earnings have consistently increased since then, with a significant jump from 2018 to 2019. However, its number of players and tournaments are much lower compared to the other games on the list.

  The number of people playing each game has varied over the years, with some games experiencing an increase and others experiencing a decline. However, all of the games on the list have a significant number of players, showing the popularity of esports as a whole.

  Overall, the data shows that esports is a growing industry with several popular titles and a significant following. While some games may experience fluctuations in earnings and popularity, the industry as a whole is expected to continue to grow in the coming years.
