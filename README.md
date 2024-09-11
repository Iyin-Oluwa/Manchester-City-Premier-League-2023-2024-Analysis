# Manchester-City-Premier-League-2023-2024-Analysis


### Introduction

The Manchester City Premier League 2023/2024 Analysis project is a comprehensive Power BI dashboard that provides a detailed examination of the team's performance throughout the season. As a Manchester City fan, I combined my passion for the team with my expertise in data analysis using Power BI to create an interactive and insightful dashboard. Leveraging various data visualizations, this project presents key insights into match outcomes, goal statistics, and comparative performance in home versus away games. Designed for fans, analysts, and coaching staff, the dashboard offers an intuitive and interactive way to explore Manchester City's journey in the EPL, making it easier to identify trends, strengths, and areas for improvement.


### Project Overview
This Power BI project provides an in-depth analysis of Manchester City's performance during the 2023/2024 English Premier League (EPL) season. The dashboard visualizes key metrics, offering insights into the team's match outcomes, goal statistics, performance at home versus away, and more.


### Key Performance Indicators (KPIs)
The analysis focuses on the following KPIs:

- Match Outcomes (Win/Draw/Loss) Breakdown: Displays the number of wins, draws, and losses, along with their respective percentages.
- Total Goals Scored vs. Conceded: Compares the total goals scored by Manchester City to the goals conceded across the season.
- Average Goals per Game: Shows the average number of goals scored per match.
- Goal Difference: Tracks the cumulative goal difference over the course of the season.
- Home vs. Away Performance: Compares the team's performance in home and away matches.
- Opposition Analysis: Breaks down goals scored and conceded against each opponent.


### DAX Analysis
Below are some key DAX measures used in the dashboard:

- Match Outcome Calculation:
```dax
Wins = COUNTROWS(FILTER('EPL', 'EPL'[OUTCOME] = "Win")) 
Draws = COUNTROWS(FILTER('EPL', 'EPL'[OUTCOME] = "Draw"))
Losses = COUNTROWS(FILTER('EPL', 'EPL'[OUTCOME] = "Lost"))
```

- Total Goals Scored:
```dax
Total Goals Scored = SUM('EPL'[GOAL_FORWARD])
```

- Total Goals Conceded:
```dax
Total Goals Conceded = SUM('EPL'[GOAL_AGAINST])
```

- Average Goals per Game:
```dax
Average Goals per Match = DIVIDE([Total Goals Scored], [Total Matches], 0) 
```

- Goal Difference:
```dax
Goal Difference = [Total Goals Scored] - [Total Goals Conceded]
```





### Visualizations

- Match Outcomes
Wins/Draws/Losses: A card visualization showing the total number of wins, draws, and losses.
Win/Draw/Loss Breakdown: A pie chart visualizing the percentage breakdown of wins, draws, and losses.

- Total Goals Scored vs. Conceded
Clustered Column Chart: Comparing the total goals scored and goals conceded across the season, with matchdays on the x-axis and the number of goals on the y-axis.

- Average Goals per Game
Card Visualization: Showing the average goals scored per match, calculated by dividing the total goals scored by the number of matches played.

- Goal Difference
Line Chart: Tracking the goal difference over the season, with matchdays on the x-axis and the goal difference on the y-axis.

- Home vs. Away Performance
Stacked Bar Chart: Comparing the results in home versus away games, filtered by the venue.

- Opposition Analysis
Table/Matrix Visualization: Showing the goals scored and conceded against each opponent, with filters for specific matchdays or venues.



![m c 1](https://github.com/user-attachments/assets/b88b5da3-ec7c-41ab-b56e-2e97c77a8af4)




![m c 2](https://github.com/user-attachments/assets/764f6363-fa60-496a-88f1-bd3a9b2e2780)




![m c 3](https://github.com/user-attachments/assets/46f8ea0a-2ac7-47e2-a6d4-cf5f7d9dca93)



### Findings
- Match Outcomes: Manchester City had a dominant season with a high percentage of wins compared to draws and losses.
- Goals Scored vs. Conceded: The team consistently outperformed opponents, scoring more goals than they conceded in most matches, showcasing their offensive strength.
- Home vs. Away Performance: Stronger performance was observed in home games compared to away matches, indicating the advantage of playing at the Etihad Stadium.
- Goal Difference: Manchester City's positive goal difference increased progressively, reflecting their strong defense and attack.
- Opposition Analysis: Certain opponents posed more challenges, but overall, the team performed exceptionally well across different matchdays.


### Data Source
The data for this project was collected from official Premier League records. 


### Tools Used
- Power BI: For data visualization and dashboard creation.
  
- Excel: For data collection and preprocessing (MANCHESTER CITY EPL 23-24.xlsx), containing matchday information, outcomes, goals scored, goals conceded, and more).


### Conclusion
This dashboard serves as a powerful tool to analyze and track the performance of Manchester City during the 2023/2024 EPL season. The insights generated can help in understanding match outcomes, goal trends, overall team performance, and for coaches to glean valuable insights into the team's strengths and areas for improvement.
