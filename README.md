# Hotel Up-selling Optimization - Data Science Project 🏨📊

## 📌 Project Overview
This project focuses on analyzing real-world, anonymized data exported from the **KWHotel** Property Management System. The primary business goal is to optimize the up-selling process (additional services like bar, restaurant, parking) at the hotel reception. By identifying which demographic groups are most likely to make additional purchases, we can move away from "blind" offering and save operational time.

## 🎯 Objectives
1. **Demographic Profiling:** Determine average additional spending across different guest segments (Family, Couple, Single, Group).
2. **Statistical Validation:** Prove whether differences in spending are statistically significant or merely random fluctuations.
3. **Predictive Modeling:** Build a Machine Learning model capable of predicting the probability of a guest purchasing additional services based on their reservation parameters.

## 🛠️ Technology Stack
* **Language:** Python
* **Data Manipulation:** `pandas`, `numpy`
* **Statistical Testing:** `scipy.stats` (ANOVA, Pearson/Spearman Correlations)
* **Machine Learning:** `scikit-learn` (Logistic Regression, One-Hot Encoding)
* **Data Visualization:** `matplotlib`, `seaborn`

## 📈 Key Business Insights
* **Families are the most profitable segment**, spending on average ~1,530 PLN on additional services.
* **Length of Stay matters:** A strong positive Spearman correlation (~0.74) indicates that every consecutive night significantly increases the likelihood of additional spending.
* **Predictive Accuracy:** The final Logistic Regression model achieved an **80% Recall rate** for the "Purchasing" class (handling imbalanced data with `class_weight='balanced'`). This means the system correctly identifies 8 out of 10 guests who are actually inclined to spend money on-site.

## 📁 Repository Structure
* `Final_Project_Hotel_English.ipynb` - The main Jupyter Notebook containing the full data pipeline: cleaning, KPI calculation, statistical testing, and the Machine Learning model.
