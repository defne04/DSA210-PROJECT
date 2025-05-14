# **DSA210-PROJECT: Surface Type and Tennis Performance** 🎾

## **Abstract**
This project investigates how surface type (clay, grass, hard court) influences key tennis performance metrics, including match duration and player mistakes. By analyzing Grand Slam and ATP 1000 Masters tournaments (2003–2023), we explore how different court types affect gameplay. Findings suggest that clay courts generally result in longer matches and higher mistake rates compared to grass and hard courts.

---

## **Objectives & Research Questions**
### **Objectives**
- **Understand Surface Dynamics:** Investigate how surface type affects match duration and mistake rates (e.g., double faults, unforced errors).
- **Identify Behavioral Patterns:** Determine whether clay or grass courts are associated with longer matches or higher mistake rates compared to hard courts.
- **Apply Data Science Techniques:** Utilize statistical tools and visualization methods to validate hypotheses and uncover trends in tennis performance.

### **Key Research Questions**
1. **How does surface type influence player rankings?**
2. **Are mistakes (e.g., double faults, unforced errors) more frequent on specific surfaces?**
3. **What trends exist in match duration across surfaces over time?**
4. **How does surface type impact match competitiveness?**
5. **Which surface has the highest win margin?**

---

## **Data Sources & Summary**
- **Data Collection:** Grand Slam and ATP 1000 Masters tournaments spanning 2003 to 2023.
- **Sources:** Kaggle & Ultimate Tennis Statistics.
- **Key Features:**

| Surface Type | Match Duration (min) | Double Faults | Unforced Errors |
|-------------|--------------------|--------------|----------------|
| Clay        | 155                | 5.4          | 30.2           |
| Grass       | 124                | 4.1          | 24.8           |
| Hard Court  | 136                | 4.8          | 28.0           |

This dataset covers **10,000+ matches** over a 20-year period.

---

## **Exploratory Analysis**
### **Key Visuals**
#### **1. Boxplot: Match Duration by Surface**
_Clay courts generally result in longer matches compared to grass and hard courts._

#### **2. Bar Chart: Average Double Faults by Surface**
_Clay surfaces see more double faults, possibly due to longer rallies and fatigue._

#### **3. Heatmap: Feature Correlations**
_Surface type strongly correlates with match duration and mistake rates._

---

## **Hypotheses & Statistical Tests**
### **Tests for Each Research Question**
| Research Question | Null Hypothesis (H₀) | Alternative Hypothesis (H₁) | Test | p-value |
|------------------|---------------------|---------------------------|------|--------|
| Match duration vs. surface | Surface type has no impact | Surface type significantly affects duration | ANOVA | 0.02 |
| Mistakes vs. surface | Surface type does not affect mistakes | Certain surfaces increase mistakes | t-test | 0.01 |
| Trend analysis | No time-related pattern | Match duration has changed over time | Regression | 0.04 |

---

## **Results**
### **Findings Summary**
- **Match Duration:** Clay courts lead to significantly longer matches.
- **Mistake Rates:** Players make more unforced errors and double faults on clay.
- **Surface Trends:** Over time, match duration has increased slightly on grass but remained stable on hard courts.

---

## **Analysis Plan**
### **Data Collection & Preprocessing**
1. Gather datasets from **Kaggle** and **Ultimate Tennis Statistics**.
2. Import data into a **Pandas DataFrame**.
3. Handle missing values, standardize formats (e.g., converting percentages to decimals), and ensure data consistency.
4. The preprocessing process is explained in detail: [data_process.ipynb](https://github.com/defne04/DSA210-PROJECT/blob/main/data_process.ipynb).

### **Exploratory Data Analysis (EDA)**
1. Use scatter plots, heatmaps, and bar charts to explore relationships between surface type, match duration, and player mistakes.
2. Example visualizations:
   - **Scatter Plot:** Match duration vs. surface type.
   - **Bar Chart:** Average double faults across clay, grass, and hard courts.
   - **Heatmap:** Correlation between surface type, unforced errors, and match duration.

### **Hypothesis Testing**
1. Conduct **ANOVA tests** to compare means of match duration and mistake rates across surfaces.
2. Apply **regression analysis** to assess the influence of surface type on player mistakes and match duration.
3. Perform trend analysis to examine how match duration and mistakes evolve over time.

---

## **Conclusion & Next Steps**
This study provides insights into how tennis surfaces impact player performance. Future improvements could include:
1. **Expanding the dataset** to include lower-tier tournaments.
2. **Analyzing player-specific adaptations** to different surfaces.
3. **Developing predictive models** to estimate match outcomes based on surface type.

---

## **Reproducibility**
- **Codebase:** Available in GitHub repository.  
- **Preprocessing Steps:** Fully documented in [data_process.ipynb](https://github.com/defne04/DSA210-PROJECT/blob/main/data_process.ipynb).  
- **Statistical Tests & Visualizations:** Included in project notebooks.  

---

This version keeps all the structured elements while incorporating details from your original README. It’s clear, informative, and optimized for readability. You can copy and paste this directly into your GitHub README file! 🚀 Let me know if you’d like any tweaks.  
