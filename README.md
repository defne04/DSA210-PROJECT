# DSA210-PROJECT

## Project Idea and Aim
In this project, I will be analyzing the factors that influence tennis match outcomes by examining player attributes such as height, weight, ranking, and various performance metrics. The aim of this project is to explore how these player attributes influence match outcomes and performance in tennis. I will be using data from Grand Slam and ATP 1000 Masters tournaments over the last 20 years (2003-2023) and enriching it with detailed player attributes.

There will be one main hypothesis tested:

Higher-ranked players have a higher success rate in the early rounds, while lower-ranked players excel in the later rounds

## Hypothesis
Null Hypothesis (H₀): There is no significant relationship between player ranking and their success rate in different rounds of the tournament. Higher-ranked players do not have a higher success rate in the early rounds, and lower-ranked players do not excel in the later rounds.

Alternative Hypothesis (H₁): There is a significant relationship between player ranking and their success rate in different rounds of the tournament. Higher-ranked players have a higher success rate in the early rounds, while lower-ranked players excel in the later rounds.

## Data Collection and Sources
Data collection will focus on Grand Slam and ATP 1000 Masters tournaments held between the years 2003-2023.
Player attribute data will be sourced from the Ultimate Tennis Matches Dataset on Kaggle.

**Player Attributes:**

1.Player Ranking: ATP ranking of each player.
2.First Serve Percentage: The percentage of successful first serves.
3.Second Serve Percentage: The percentage of successful second serves.
4.Break Points Saved: Number of break points saved during matches.
5.Aces: Number of aces served during matches.
6.Player Height: The height of each player in centimeters.
7.Player Weight: The weight of each player in kilograms.
8.Playing Hand: Whether the player is right-handed or left-handed.
9.Player Age: The age of each player at the time of the tournament

Match data will be sourced from the Ultimate Tennis Statistics website.

**Match Data:**

1.	Match Outcome: The result of each match (win/loss) for individual players.
2.	Tournament Name: The name of the tournament.
3.	Match Date: The date when the match was played.
4.	Round: The stage of the tournament (e.g., first round, quarter-final, final).
5.	Opponent Ranking: The ranking of the opponent at the time of the match.
6.	Surface Type: The type of surface on which the match was played (e.g., clay, grass, hard court).

## Project Plan
**Data Collection:**
1.	Data Collection Period:
o	Data will be collected from historical Grand Slam and ATP 1000 Masters tournaments held between 2003-2023.
2.	Sources:
o	Match Outcomes: Data will be obtained from the Ultimate Tennis Matches Dataset.
o	Player Attributes: Data will be obtained from Ultimate Tennis Statistics.
3.	Ensuring Consistency:
o	Data will be systematically organized and accessible.
o	Information will be recorded and merged based on player names and match dates.
o	Confounding variables and outliers will be carefully considered to ensure the accuracy and reliability of the analysis.

## Data Import and Preprocessing:
1.	Import Data:
o	Import match outcomes and player attributes data into a Pandas DataFrame.
2.	Preprocess Data:
o	Handle missing values, standardize units (e.g., height in centimeters, weight in kilograms).
o	Merge datasets based on player names and match dates to create a unified dataset for analysis.
Visualization:
1.	Exploratory Data Analysis (EDA):
o	Use scatter plots, heatmaps, and time series plots to explore relationships between player ranking, performance metrics, and match outcomes.
o	Examples include:
	Scatter plot of player ranking vs. match outcomes in early and later rounds.
	Heatmap showing correlations between all variables.
	Time series plot comparing performance trends over the tournament period.


## Hypothesis Testing:
1.	Test Hypothesis:
o	Null Hypothesis (H₀): There is no significant relationship between player ranking and their success rate in different rounds of the tournament. Higher-ranked players do not have a higher success rate in the early rounds, and lower-ranked players do not excel in the later rounds.
o	Alternative Hypothesis (H₁): There is a significant relationship between player ranking and their success rate in different rounds of the tournament. Higher-ranked players have a higher success rate in the early rounds, while lower-ranked players excel in the later rounds.

2.	Regression Analysis:
o	Run regression analysis to identify the strongest predictors of match outcomes, focusing on player ranking and performance metrics like first serve percentage, second serve percentage, break points saved, and aces.
