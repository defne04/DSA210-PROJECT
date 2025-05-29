# **DSA210-PROJECT: Surface Type and Tennis Performance** 🎾  

## **Abstract**  
This project investigates the impact of tennis court surfaces (**clay, grass, hard court**) on match duration and player mistakes. By analyzing **Grand Slam and ATP 1000 Masters** tournaments from **2003 to 2023**, we examine long-term trends and behavioral patterns among players. Findings indicate that **clay courts lead to longer matches and higher mistake rates**, while **grass surfaces favor faster-paced games with lower mistake counts**.  

---

## **Contents**  
- [Objectives & Research Questions](#objectives--research-questions)  
- [Data Sources & Summary](#data-sources--summary)  
- [Exploratory Analysis](#exploratory-analysis)  
- [Hypotheses & Statistical Tests](#hypotheses--statistical-tests)  
- [Results](#results)  
- [Conclusion & Next Steps](#conclusion--next-steps)  
- [Reproducibility](#reproducibility)  

---

## **Objectives & Research Questions**  

### **Objectives**  
- Understand the **impact of surface type** on match dynamics.  
- Identify **patterns in ranking differences** between players on different surfaces.  
- Apply **machine learning techniques** to predict match duration based on surface type and player statistics.  

### **Key Research Questions**  
1. How does **match intensity** vary by surface?  
2. Does surface type affect **ranking imbalance** between Player 1 and Player 2?  
3. What are **long-term trends** for different surfaces?  
4. Do certain surfaces lead to **longer matches**?  
5. Which surface type results in **higher or lower win margins**?  

---

## **Data Sources & Summary**  

### **Dataset Overview**  
- **Tournaments Covered:** Grand Slam & ATP 1000 Masters (**2003–2023**)  
- **Total Matches:** **10,000+**  
- **Data Sources:** Kaggle, Ultimate Tennis Statistics  

### **Matches per Surface**  

| Surface Type | Total Matches | Years Covered |  
|-------------|--------------|--------------|  
| **Clay**    | ~4,000       | 2003–2023    |  
| **Grass**   | ~1,500       | 2003–2023    |  
| **Hard**    | ~4,500       | 2003–2023    |  

### **Key Features**  

| Feature               | Description                                      |  
|----------------------|------------------------------------------------|  
| **Surface Type**     | Clay, Grass, Hard                              |  
| **Match Duration (min)** | Total match time in minutes                  |  
| **Double Faults**    | Number of double faults committed              |  
| **Unforced Errors**  | Player mistakes (unforced errors count)        |  
| **Player 1 / Player 2 Rank** | ATP rankings at match time             |  

---

## **📊 Exploratory Analysis**  

### **Key Visuals**  

#### **Match Intensity by Surface**
_Clay courts generally result in longer matches compared to grass and hard courts._

![](match_indensity.png)

#### **Player Rankings by Surface**
_Compared average rankings of Player 1 and Player 2 across surfaces. Clay courts tend to attract higher-ranked matchups, while hard courts show more ranking variability._

![](player1_ranking.png)
![](player2_ranking.png)

#### **Surface Trends Over Time**
_Hard courts dominate the professional circuit, but the share of clay court matches has shown relative stability. Grass courts remain the least common._

![](surface_trends.png)
![](surface_trends2.png)

#### **Average Win Margin by Surface**
_Matches on clay courts have closer scorelines on average, suggesting more competitive encounters, whereas grass surfaces often result in higher win margins due to faster pace and serve-dominated play._

![](average_win.png)

---

## **Hypotheses & Statistical Tests**  

### **Test Summary**  

| Research Question | Null Hypothesis (H₀) | Alternative Hypothesis (H₁) | Test | p-value |  
|------------------|---------------------|---------------------------|------|--------|  
| Surface vs. Match Duration | Surface type does not affect duration | Surface type significantly affects duration | ANOVA | **0.02** |  
| Surface vs. Mistakes | Surface type does not impact mistakes | Certain surfaces lead to more mistakes | t-test | **0.01** |  
| Surface Trends | No time-related pattern | Match duration has changed over time | Regression | **0.04** |  

### **Findings Summary**  
 **Clay courts** result in significantly **longer matches**.  
 Players commit **more unforced errors** and **double faults on clay**.  
 **Match duration** has **slightly increased on grass** over time but remained stable on hard courts.  

---

## **Results**  

### **Example Predictions from Machine Learning Model**  

| Surface | Player 1 Rank | Player 2 Rank | Predicted Match Duration (sets) |  
|--------|---------------|---------------|---------------------------------|  
| **Clay** | 5 | 15 | **4.2** |  
| **Grass** | 20 | 30 | **3.1** |  
| **Hard Court** | 12 | 14 | **3.8** |  

### **Model Details**  
- **Algorithm:** Random Forest Regressor  
- **Train/Test Split:** 80% training, 20% testing  
- **Evaluation Metrics:**  
  - **Mean Absolute Error (MAE):** `0.67 sets`  
  - **Root Mean Squared Error (RMSE):** `0.86 sets`  

---

## **Conclusion & Next Steps**  

This study confirms that **surface type significantly influences match duration and mistake rates**, with clay courts resulting in **longer, more error-prone matches**. Future improvements may include:  
1. Expanding the dataset to include **lower-tier tournaments**.  
2. Analyzing **player-specific adaptations** to surfaces.  
3. Enhancing **machine learning models** for **more precise duration predictions**.  

---

## **Reproducibility**  
- **Data Processing Notebook:** [data_process.ipynb](https://github.com/defne04/DSA210-PROJECT/blob/main/data_process.ipynb)  
- **Machine Learning Model Notebook:** [ML_model.ipynb](https://github.com/defne04/DSA210-PROJECT/blob/main/ML_model.ipynb)  

  
