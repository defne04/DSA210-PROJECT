# DSA210-PROJECT

## Project Idea and Aim
In this project, I will be analyzing the factors that influence tennis match outcomes by examining player attributes such as height, weight, ranking, and various performance metrics. The aim of this project is to explore how these player attributes influence match outcomes and performance in tennis. I will be using data from Grand Slam and ATP 1000 Masters tournaments over the last 20 years (2003-2023) and enriching it with detailed player attributes.

There will be one main hypothesis tested:

**Higher first serve percentages give a higher rate of match wins**

## Hypothesis
**Null Hypothesis (H₀):** There is no significant relationship between a player's first serve percentage and their match win rate. Higher first serve percentages do not significantly affect the rate of match wins.

**Alternative Hypothesis (H₁):** There is a significant relationship between a player's first serve percentage and their match win rate. Higher first serve percentages significantly increase the rate of match wins.

## Data Collection and Sources
Data collection will focus on Grand Slam and ATP 1000 Masters tournaments held between the years 2003-2023.
Player attribute data will be sourced from the Ultimate Tennis Matches Dataset on Kaggle.

**Player Attributes:**

1. First Serve Percentage: The percentage of successful first serves.
2. Player Ranking: ATP ranking of each player.
3. Second Serve Percentage: The percentage of successful second serves.
4. Break Points Saved: Number of break points saved during matches.
5. Aces: Number of aces served during matches.
6. Player Height: The height of each player in centimeters.
7. Player Weight: The weight of each player in kilograms.
8. Playing Hand: Whether the player is right-handed or left-handed.
9. Player Age: The age of each player at the time of the tournament

Match data will be sourced from the Ultimate Tennis Statistics website.

**Match Data:**

1. Match Outcome: The result of each match (win/loss) for individual players.
2. Tournament Name: The name of the tournament.
3. Match Date: The date when the match was played.
4. Round: The stage of the tournament (e.g., first round, quarter-final, final).
5. Opponent Ranking: The ranking of the opponent at the time of the match.
6. Surface Type: The type of surface on which the match was played (e.g., clay, grass, hard court).

## Project Plan
### Data Collection:
1. **Data Collection Period:**
   - Data will be collected from historical Grand Slam and ATP 1000 Masters tournaments held between 2003-2023.

2. **Sources:**
   - Match Outcomes: Data will be obtained from the Ultimate Tennis Matches Dataset.
   - Player Attributes: Data will be obtained from Ultimate Tennis Statistics.

3. **Ensuring Consistency:**
   - Data will be systematically organized and accessible.
   - Information will be recorded and merged based on player names and match dates.
   - Confounding variables and outliers will be carefully considered to ensure the accuracy and reliability of the analysis.

### Data Import and Preprocessing:
1. **Import Data:**
   - Import match outcomes and player attributes data into a Pandas DataFrame.

2. **Preprocess Data:**
   - Handle missing values, standardize units (e.g., height in centimeters, weight in kilograms).
   - Merge datasets based on player names and match dates to create a unified dataset for analysis.

### Visualization:
**Exploratory Data Analysis (EDA):**
1. Use scatter plots, heatmaps, and time series plots to explore relationships between first serve percentage, performance metrics, and match outcomes.
2. Examples include:
   - Scatter plot of first serve percentage vs. match win rate.
   - Heatmap showing correlations between all variables.
   - Time series plot comparing performance trends over the tournament period.

## Hypothesis Testing:
1. **Test Hypothesis:**
   - Null Hypothesis (H₀): There is no significant relationship between a player's first serve percentage and their match win rate. Higher first serve percentages do not significantly affect the rate of match wins.
   - Alternative Hypothesis (H₁): There is a significant relationship between a player's first serve percentage and their match win rate. Higher first serve percentages significantly increase the rate of match wins.

2. **Regression Analysis:**
   - Run regression analysis to identify the strongest predictors of match outcomes, focusing on first serve percentage and other performance metrics.

## Conclusion
By the end of this project, I hope to answer the following questions:
- Does first serve percentage significantly influence match win rates?
- Which performance metrics are key predictors of match wins?
- What are the key factors that predict match outcomes in ATP tournaments?

This project aims to leverage data science to gain insights into tennis performance, providing valuable information for players, coaches, and analysts. Understanding the factors behind match outcomes is key to optimizing strategies and achieving success in sports and beyond.

Through this analysis, I will apply the concepts learned in my data science course to a real-world scenario. The findings from this project will contribute to developing targeted training practices and match strategies, ultimately improving tennis performance.
