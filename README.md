#Google Play Store Apps Analysis
## 📌 Project Overview
This project analyzes a dataset of apps from the Google Play Store. The goal was to clean the raw data, create meaningful KPIs, 
and build visualizations that highlight trends in installs, ratings, categories, and revenue potential.

## Dataset
- Source: Google Play Store dataset (CSV file with ~9,600 rows and 14 columns).
- Key Columns:
- App – App name
- Category – App category (e.g., Games, Tools, Business)
- Rating – Average user rating
- Reviews – Number of reviews (not used in KPIs here)
- Size – App size in MB
- Installs – Number of installs (cleaned from strings like “1,000+”)
- Type – Free or Paid
- Price – Price of the app (converted to numeric)
- Content Rating – Age group suitability
- Last Updated – Date of last update
  
## Data Preparation
Steps taken to prepare the dataset:
- Removed duplicates and dropped unnecessary index column.
- Cleaned Installs (removed “+” and “,”, converted to integer).
- Cleaned Price (removed “$”, replaced “Free” with 0, converted to float).
- Converted Last Updated to datetime.
- Filled missing values in Rating (mean), Size (median), and version columns (Unknown).
  
## KPIs
- Total unique apps
- Average rating across apps
- Total installs
- Free vs Paid app counts
- Estimated revenue = Price × Installs (for Paid apps)
  
## Visualizations
- Top 10 Categories by Installs
- Top 10 Categories by Average Rating
- Top 10 Revenue Generating Apps
- Correlation Heatmap (Rating, Size, Installs, Price, Revenue)
  
## Insights
- Free apps dominate the store compared to paid apps.
- Certain categories (like Games and Tools) drive the majority of installs.
- Paid apps generate revenue potential, but only a small fraction of apps are paid.
- Average ratings are fairly high across categories, with some categories consistently outperforming others.
