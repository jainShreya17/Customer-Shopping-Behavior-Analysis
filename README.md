# Customer-Shopping-Behavior-Analysis
An end-to-end data analytics project utilizing Python (Pandas) for EDA, MySQL for business querying, and Power BI for interactive dashboarding to uncover insights from 3,900 customer transactions.
## Overview
The primary objective is to transform raw transactional data into actionable business intelligence. The project explores key metrics such as revenue distribution by gender and age, the impact of subscription status on spending, and product-specific performance across different categories.
## Dataset:
 3,900 rows and 18 columns.
 Demographics: Age, Gender, Location, and Subscription Status.
 Transaction Details: Item Category, Purchase Amount, Season, Size, and Color.
 Behavioral Data: Review Ratings, Shipping Type, and Discount/Promo usage.
 ## Tools Used : 
 Data Cleaning & EDA: Python (Pandas).
 Database Management: MySQL.
 Data Visualization: Power BI.
 Presentation: Gamma AI (for PPT generation) and Microsoft Word (for reporting).
 ## Project Steps
 1. **Data Preparation (Python)Exploration**: Conducted initial checks using **df.info()** and **describe()** to understand data structure and statistics.
 *Cleaning*: Imputed 37 missing values in the "Review Rating" column using the category-specific median.
 *Standardization*: Converted column names to snake_case for consistency.
 *Feature Engineering*: Created an age_group column by binning ages and a purchase_frequency_days column.
 2. **Structured Analysis (SQL)** : The cleaned data was loaded into MySQL to perform complex business queries:
 Revenue Analysis: Found that Male customers generated significantly higher revenue ($157,890) compared to Female customers ($75,191).
 *Customer Segmentation*: Classified users into Loyal (3,116), Returning (701), and New (83) segments.
 *Shipping Impact*: Identified that "Express" shipping users spend slightly more on average ($60.48) than "Standard" shipping users ($58.46).
 3. **Data Visualization (Power BI)** : Developed an interactive Customer Behavior Dashboard highlighting:
 *KPIs*: Total customers (3.9K), average purchase amount ($59.76), and average review rating (3.75).
 *Subscription Trends*: 27% of customers are subscribers, while 73% are not.
 *Category Performance*: "Clothing" emerged as the top category for both sales volume and revenue.
 ## Key Results & RecommendationsTargeted Marketing:
  Focus campaigns on Young Adults, as they are the highest revenue-contributing age group ($62,143).
  **Loyalty Programs**: Reward the 3,116 "Loyal" customers to maintain retention and incentivize "New" customers to move into the "Returning" segment.
  **Subscription Push**: Only 27% of users are subscribers; promoting exclusive benefits could bridge the gap, as subscribers and non-subscribers currently have very similar average spends (~$59).
  **Product Highlighting**: Gloves, Sandals, and Boots are the highest-rated products and should be featured in promotional content.
  ## How to RunPython:
   Run the **Jupyter Notebook** or **.py** script to clean the data and export the cleaned_shopping_data.csv.
   **SQL**: Import the cleaned CSV into a **MySQL** database and run the queries provided in the analysis_queries.sql file.
   **Power BI**: Open the .pbix file to view the interactive dashboard. Ensure the data source is updated to point to your local database or CSV file.
