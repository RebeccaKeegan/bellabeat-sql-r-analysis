# 📊 Bellabeat Smart Device Usage – SQL & R Analysis

## 🧩 Overview  
This project analyzes smart device usage data to uncover patterns in activity and sleep among users, inspired by Bellabeat’s wellness tracking products. By leveraging SQL for data management and R for statistical analysis and visualization, we generate actionable insights to support product development and marketing strategies.

## 🗃️ Dataset  
- **Source**: [FitBit Fitness Tracker Data on Kaggle](https://www.kaggle.com/datasets/arashnic/fitbit)  
- **Files Used**:  
  - `daily_activity.csv` – activity, steps, calories, sedentary minutes  
  - `sleep_day.csv` – sleep duration and time in bed  
- **Limitations**:  
  - Small sample size (30 users)  
  - Primarily female demographic  
  - Incomplete sleep tracking for some users  

## 🛠️ Tools Used  
- **SQL** (SQLite) for data loading, filtering, and joins  
- **R** (tidyverse, ggplot2, corrplot) for analysis and visualization  

## ❓ Business Questions  
- Is there a relationship between physical activity and sleep duration?  
- How sedentary are users despite their activity levels?  
- What behavioral patterns can inform product or app engagement strategies?  

## 🔍 Methodology  
### SQL Workflow  
- Created tables for activity and sleep data  
- Joined datasets on user ID and date  
- Filtered and exported merged results for R-based analysis  

### R Workflow  
- Imported SQL-joined dataset using `DBI`  
- Conducted exploratory data analysis (EDA)  
- Built scatter plots and correlation matrices  
- Summarized trends in physical and sleep behavior  

## 📈 Key Findings  
- Weak-to-moderate positive correlation between steps taken and minutes asleep  
- Most users are still sedentary for long periods despite moderate daily steps  
- Sleep data was only consistently recorded for about 25% of total days  

![Steps vs Sleep](visuals/steps_vs_sleep.png)  
*Scatter plot showing relationship between steps and sleep duration*

![Correlation Plot](visuals/corr_plot.png)  
*Correlation matrix between activity, calories, and sleep metrics*

## 📌 Recommendations  
- Introduce sleep tracking reminders or gamification to boost consistency  
- Promote short, high-impact activities for sedentary users  
- Emphasize recovery and sleep features in marketing to health-conscious users  
