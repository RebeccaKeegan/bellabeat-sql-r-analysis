# 📊 Bellabeat Smart Device Usage – BigQuery & Tableau Analysis

## 🧩 Overview  
This project explores smart device usage data to uncover trends in user activity and sleep, inspired by Bellabeat’s wellness products. Using Google BigQuery for scalable SQL analysis and Tableau for interactive dashboards, the goal is to surface insights that can support data-driven product and marketing decisions.

## 🗃️ Dataset  
- **Source**: [FitBit Fitness Tracker Data on Kaggle](https://www.kaggle.com/datasets/arashnic/fitbit)  
- **Files Used**:  
  - `daily_activity.csv` – steps, calories, sedentary minutes  
  - `sleep_day.csv` – sleep duration and time in bed  
- **Limitations**:  
  - Small sample size (30 users)  
  - Primarily female demographic  
  - Incomplete sleep tracking coverage  

## 🛠️ Tools Used  
- **Google BigQuery** – for querying and joining large structured datasets  
- **Tableau** – for building interactive dashboards and data storytelling  

## ❓ Business Questions  
- What’s the relationship between physical activity and sleep?  
- How much time do users spend sedentary, and how does this vary by day?  
- What insights can drive product features or marketing campaigns?  

## 🔍 Methodology  
### BigQuery Workflow  
- Uploaded CSVs to Google Cloud Storage and imported into BigQuery  
- Wrote SQL to clean and join activity and sleep datasets on user ID and date  
- Aggregated daily metrics and exported summary views for Tableau  

### Tableau Workflow  
- Connected Tableau to BigQuery export  
- Built dashboards including:
  - Steps vs Sleep scatter plots  
  - Average activity by weekday  
  - Sedentary time distribution  
  - Correlation heatmap (using calculated fields)  

## 📈 Key Findings  
- Moderate correlation between daily step count and total minutes asleep  
- Sedentary behavior remains high, even on active days  
- Sleep data logging is inconsistent across users  

![Example Dashboard](visuals/tableau_dashboard_preview.png)  
*Example dashboard showing step vs sleep relationships and daily patterns*
