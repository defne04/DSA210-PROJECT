# **DSA210-PROJECT: Surface Type and Tennis Performance** 🎾

## **Project Overview**
This project investigates how surface type (clay, grass, hard court) influences key tennis performance metrics. Specifically, I aim to uncover whether players tend to stay longer in matches and make more mistakes (e.g., double faults, unforced errors) on certain surfaces. By analyzing match duration, player mistakes, and surface types, I will explore the ways different court types affect gameplay.

The approach includes gathering data on match duration and errors across surfaces, exploring patterns using statistical tools, and testing hypotheses to identify surface-specific challenges. The findings will provide actionable insights for optimizing strategies tailored to different court types.

---

## **Objectives**
### *Understand Surface Dynamics*
- Investigate how surface type affects match duration and mistake rates (e.g., double faults, unforced errors).

### *Identify Behavioral Patterns*
- Determine whether certain surfaces, like clay and grass, are associated with longer matches or higher mistake rates compared to hard courts.

### *Apply Data Science Techniques*
- Utilize data analysis and visualization methods to validate hypotheses and uncover trends in tennis performance.

---

## **Dataset**
### *Data Collection Sources*
- Data will be collected from **Grand Slam and ATP 1000 Masters tournaments** spanning from 2003 to 2023.
- Player performance data and match statistics will be sourced from **Kaggle** and **Ultimate Tennis Statistics**.

### **Features Tracked**
#### Player Attributes
1. **First Serve Percentage**: Percentage of successful first serves.
2. **Second Serve Percentage**: Percentage of successful second serves.
3. **Double Faults**: Number of double faults committed during a match.
4. **Unforced Errors**: Number of unforced errors recorded.
5. **Break Points Saved**: Number of break points saved.
6. **Break Points Converted**: Percentage of break points successfully converted.
7. **Aces**: Number of aces served.
8. **Return Percentage**: Percentage of successful returns against opponent serves.
9. **First Serve Speed**: Average speed of the player’s first serves in km/h.
10. **Second Serve Speed**: Average speed of the player’s second serves in km/h.
11. **Service Games Won**: Percentage of service games the player won.
12. **Return Games Won**: Percentage of return games the player won.
13. **Player Ranking**: ATP ranking of each player.

#### Match Data
1. **Match Outcome**: Whether the match was won or lost.
2. **Match Duration**: Total match length (in minutes).
3. **Surface Type**: The surface on which the match was played (clay, grass, hard court).
4. **Tournament Name**: Name of the tournament.

---

## **Hypothesis**
### Null Hypothesis (H₀):
Surface type does not significantly influence match duration or the frequency of player mistakes (e.g., double faults, unforced errors).

### Alternative Hypothesis (H₁):
Surface type significantly influences match duration and the frequency of player mistakes (e.g., double faults, unforced errors).

---

## **Tools and Technologies**
I will utilize the following tools for data analysis and visualization:
1. **Python**: For data preprocessing, statistical analysis, and visualization.
2. **Pandas**: To manipulate and clean datasets.
3. **Matplotlib and Seaborn**: To create visualizations like scatter plots, bar charts, and heatmaps.
4. **SciPy**: For hypothesis testing and regression analysis.

---

## **Analysis Plan**
### *Data Collection and Preprocessing*
1. Gather datasets from **Kaggle** and **Ultimate Tennis Statistics**.
2. Import data into a Pandas DataFrame.
3. Handle missing values, standardize formats (e.g., converting percentages to decimals), and ensure data consistency.
4. The preprocessing process of data is further explained in the following: [./data_process.ipynb](https://github.com/defne04/DSA210-PROJECT/blob/main/data_process.ipynb)

### *Exploratory Data Analysis (EDA)*
1. Use scatter plots, heatmaps, and bar charts to explore relationships between surface type, match duration, and player mistakes.
   - Examples:
     - **Scatter Plot**: Match duration vs. surface type.
     - **Bar Chart**: Average double faults across clay, grass, and hard court surfaces.
     - **Heatmap**: Correlation between surface type, unforced errors, and match duration.

### *Hypothesis Testing*
1. Test the hypothesis:
   - **Null Hypothesis (H₀):** Surface type does not significantly affect match duration or player mistakes.
   - **Alternative Hypothesis (H₁):** Surface type significantly impacts match duration and player mistakes.
2. Perform **ANOVA tests** to compare means of match duration and mistake rates across surfaces.
3. Use **regression analysis** to assess the influence of surface type on player mistakes and match duration.

### *Trend Analysis*
1. Analyze trends in match duration and mistakes across different surfaces over time.
2. Investigate correlations between **player ranking** and mistake rates for matches on clay, grass, and hard court surfaces.

---

## **Example Analysis**
### To Illustrate:
- Create a **scatter plot** comparing match duration on clay, grass, and hard court surfaces. This will highlight whether clay leads to longer matches due to slower rally speeds.
- Use a **bar chart** to compare average double faults across surfaces, identifying whether grass courts introduce more serving errors due to their unpredictability.
- Develop a **heatmap** to visualize correlations between unforced errors, match duration, and surface type.

---
## **Research Questions**
This project seeks to explore the following research questions:

1. **How does surface type influence player rankings?**
2. **Are mistakes (e.g., double faults, unforced errors) more prevalent on specific surfaces like clay or grass compared to hard courts?**
3. **What trends exist across surfaces over time?**
4. **How does surface type impact match competitiveness?**
5. **Which surface has the highest win margin?**

This project showcases the role of data science in analyzing sports performance, providing insights that can guide players and coaches to optimize their strategies based on court conditions.
