# Market_Sentiment_Analysis
---
ShopEasy, an online retail business, is facing reduced customer engagement and conversion rates despite launching several new online marketing campaigns. They are reaching out to you to help conduct a detailed analysis and identify areas for improvement in their marketing strategies.
---

Key Points:
* Reduced Customer Engagement: The number of customer interactions and engagement with the site and marketing content has declined.
* Decreased Conversion Rates: Fewer site visitors are converting into paying customers.
* High Marketing Expenses: Significant investments in marketing campaigns are not yielding expected returns.
* Need for Customer Feedback Analysis: Understanding customer opinions about products and services is crucial for improving engagement and conversions.
---
Project Overview
This project analyzes market sentiment using SQL Server, Python, and Power BI. The goal was to extract meaningful insights from customer reviews and other data sources by performing sentiment analysis and visualizing trends.
---
Technologies Used
- SQL Server (Data Storage, Cleaning, Transformation)

- Python (pyodbc, nltk, SentimentIntensityAnalyzer, VADER Lexicon for sentiment analysis)

- Power BI (Data Visualization, DAX for calculations)
---
### Approach
1. Data Loading & Cleaning (SQL Server)
 - Loaded the .bak file into SQL Server.

- Performed data cleaning using SQL queries:

- Removed null values, Transformed data (trimming whitespaces, splitting columns, converting data types)

- These transformations were later used in Power BI to ensure clean data ingestion.
---

2. Sentiment Analysis (Python)
 - Connected SQL Server to Python using pyodbc.

- Used nltk, SentimentIntensityAnalyzer, and VADER Lexicon to analyze sentiment in the customer_review table.

- Computed sentiment scores, categorized them into buckets (positive, neutral, negative).

- Saved the processed data as a CSV for further analysis.
---
3. Visualization & Reporting (Power BI)
- Loaded SQL Server tables into Power BI using queries to minimize transformations in Power BI.

- Created an interactive dashboard with four pages:
 
- Overview – High-level insights and key metrics, Conversion Details – Customer conversion trends and performance metrics, Social Media Details – Engagement and sentiment trends from social media data, Customer Review Details – Sentiment distribution and key feedback points.

- Used DAX to create calculated measures for advanced analysis.





