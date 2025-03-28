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
![image](https://github.com/Vetri2509/Market_Sentiment_Analysis/blob/main/images/Screenshot%202025-03-27%20182232.png)
- Loaded SQL Server tables into Power BI using queries to minimize transformations in Power BI.

- Created an interactive dashboard with four pages:
 
- Overview – High-level insights and key metrics, Conversion Details – Customer conversion trends and performance metrics, Social Media Details – Engagement and sentiment trends from social media data, Customer Review Details – Sentiment distribution and key feedback points.

- Used DAX to create calculated measures for advanced analysis.
---

### Insights
1. There is a decline in overall social media engagement, with views dropping throughout the year.
2. Customer ratings have remained consistent, averaging around 3.7 throughout the year.
3. May experienced the lowest overall conversion rate at 4.3%, January recorded the highest overall conversion rate at 18.5%
4. Views peaked in February and July but declined from August, Clicks and likes remained consistently low compared to views
5. The majority of customer reviews are in the higher ratings, with 140 reviews at 4 stars and 135 reviews at 5 stars, indicating overall positive feedback. Positive sentiment dominates with 275 reviews, reflecting a generally satisfied customer base. Negative sentiment is present in 82 reviews, with a smaller number of mixed and neutral sentiments, suggesting some areas for improvement but overall strong customer approval.

---
### Key Takeaways
- Pre-cleaning data in SQL Server before loading into Power BI improves performance and reduces redundancy.

- Python-based sentiment analysis provides deeper insights into customer feedback.

- This was my first-ever NLP/ML project in Python, and I learned how to use nltk for sentiment analysis.

- Well-structured Power BI dashboards enhance decision-making by making insights easily accessible.













