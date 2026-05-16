# Engagement Analytics and Correlation Deep-Dive on YouTube Trending Data

---

# 📌 Project Overview

This project performs a complete engagement analytics and correlation analysis on YouTube Trending Videos data.

The analysis focuses on audience interaction behavior, engagement performance, category benchmarking, publishing patterns, and content strategy insights using professional data analytics techniques.

The project was built entirely using:

- pandas
- matplotlib
- seaborn

---

# 📂 Dataset Information

Datasets Used:

- USvideos.csv
- US_category_id.json

Dataset Size:

- Approximately 40,949 rows
- 16 primary columns

The category JSON file was parsed successfully to map:

category_id → category_name

---

# 🛠 Methodology

Project Workflow:

1. Data Loading
2. Data Exploration
3. Data Cleaning
4. Duplicate Removal
5. Datetime Conversion
6. JSON Category Mapping
7. Feature Engineering
8. Correlation Analysis
9. Category Benchmarking
10. Audience Segmentation
11. Weekday Trend Analysis
12. Visualization & Strategic Insights

Only the first trending appearance per video_id was retained to avoid duplicated trend exposure bias.

---

# 📊 Engineered Metrics

## Engagement Rate

(likes + dislikes + comment_count) / views × 100

---

## Like Rate

likes / views × 100

---

## Dislike Rate

dislikes / views × 100

---

## Days to Trend

trending_date - publish_time

Measured in days.

---

## Publish Weekday

Extracted from publish_time to evaluate publishing performance trends.

---

# 🔗 Correlation Findings

Key Pearson Correlation Findings:

- Strong positive relationship between views and likes:
  - r ≈ 0.84

- Strong relationship between dislikes and comment_count:
  - r ≈ 0.71

- Weak positive relationship between tag count and views:
  - r ≈ 0.18

The analysis indicates that highly viewed videos tend to generate significant interaction activity, but not always proportional engagement rates.

---

# 📈 Category Benchmarking Summary

## Highest Average Engagement Rate

- News & Politics (~6.8%)

This category generated the strongest audience interaction rates.

---

## Highest Average Views

- Music (~12.4M)

Music videos dominated platform exposure and audience reach.

---

## Important Observation

Despite generating the highest views, the Music category maintained below-average engagement rates, indicating stronger passive audience behavior.

---

# 📅 Weekday Publishing Findings

Publishing weekday analysis showed measurable differences in audience exposure and interaction.

Key finding:

- Monday trending videos showed the lowest engagement levels.

This suggests audience responsiveness may vary depending on publishing timing.

---

# 👥 Audience Behavior Findings

Two audience behavior groups were identified:

## Passive Audience Videos

- High views
- Low engagement

These videos achieved strong exposure but weaker audience interaction.

---

## Niche Loyal Audience Videos

- Lower views
- Higher engagement

These videos demonstrated highly loyal and interactive audience communities despite smaller reach.

---

# 🏆 Top Trending Video Findings

Top trending videos were identified using total views.

Metrics included:

- Title
- Category
- Views
- Engagement Rate
- Days to Trend

The analysis highlighted that rapid trending performance does not always guarantee stronger engagement quality.

---
