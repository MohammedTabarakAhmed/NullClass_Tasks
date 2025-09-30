# Google Play Store Apps Analysis
## 📌 Project Overview
This project analyzes a dataset of apps from the Google Play Store. The goal was to clean raw data, create meaningful KPIs, and build visualizations that highlight trends in installs, ratings, categories, and revenue potential.

## 📂 Dataset
- Source: Google Play Store dataset (~9,600 rows, 14 columns)
- Key columns: App, Category, Rating, Size, Installs, Type, Price, Content Rating, Last Updated

## 🧹 Data Preparation
- Removed duplicates and dropped index column
- Cleaned Installs and Price columns
- Converted Last Updated to datetime
- Filled missing values in Rating (mean), Size (median), and Version (Unknown)

## 📊 KPIs
- Total unique apps
- Average rating
- Total installs
- Free vs Paid app counts
- Estimated revenue = Price × Installs (Paid apps only)

## 📈 Visualizations
- Top 10 Categories by Installs
- Top 10 Categories by Average Rating
- Top 10 Revenue Generating Apps
- Correlation Heatmap (Rating, Size, Installs, Price, Revenue)

## 🔍 Insights
- Free apps dominate the store
- Games and Tools drive most installs
- Paid apps offer revenue potential but are few
- Some categories consistently outperform in ratings

## 📊 Power BI Dashboard
An interactive Power BI report is included for deeper exploration.
- File: task1.pbix
- Tool: Power BI Desktop
- Description: Visual dashboard covering installs, ratings, revenue, and category trends
- To view: Download and open in Power BI Desktop
