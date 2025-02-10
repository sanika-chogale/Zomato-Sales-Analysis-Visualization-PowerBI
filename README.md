# Zomato Sales Analysis & Visualization in Power BI

This project is focused on analyzing Zomato sales data using Power BI. The analysis includes exploring sales trends, customer preferences, and revenue distribution through interactive visualizations. The insights aim to support data-driven decisions that enhance customer experience, optimize operations, and drive business growth.

## Objective
The objective of this project is to build a comprehensive Power BI dashboard for analyzing Zomato sales data. By examining sales performance, category preferences, and customer demographics, the goal is to uncover actionable insights that enable better strategic planning and operational efficiency.

## Relationship Model 
![Image](https://github.com/user-attachments/assets/6ce52af6-40d3-49cf-9db2-72010f5a55b7)
## Zomato Sales Data Analysis and Dashboard Creation :
Here’s a step-by-step guide for creating a Zomato Sales Dashboard in Power BI, covering data download, cleaning, transformation, and visualization:

#### Step 1: Download Data from Kaggle
- Visit Kaggle and search for a Zomato Sales Dataset or relevant datasets (e.g., food delivery, restaurant reviews, or sales trends).
- Download the dataset (usually in CSV format).
- Extract the files and save them to a folder on your system.


#### Step 2: Load Data into Power BI
- Open Power BI Desktop.
- Click on Home > Get Data > Text/CSV to load the dataset files (e.g., Sales.csv, Restaurants.csv, Customers.csv).
- Preview the data and click Load for each file you need.

#### Step 3: Clean Data Using Power Query
- Click on Transform Data to open the Power Query editor.
- Perform the following transformations:
- Remove Duplicates: Clean the data by removing duplicate entries.
- Handle Missing Values: Replace nulls in numeric fields with 0, and text fields with "Unknown."
- Rename Columns: Ensure column names are clear (e.g., Rest_ID to Restaurant ID).
- Change Data Types: Assign correct data types to columns, such as date, text, or numbers.
- Click Close & Apply to load the cleaned data back into Power BI.

#### Key Calculations in DAX
#### Total Revenue: 

```Total Revenue = SUMX(orders, orders[Sales Quantity] * orders[Sales(INR)])```

This calculation multiplies the sales quantity with the sales amount for each record and sums up the results to get the total revenue.


#### Average Rating:

```AverageRating = CALCULATE(AVERAGE('restaurant'[rating]), restaurant[rating] <> 0)```

This measure calculates the average customer rating, excluding records where the rating is zero.

#### Step 4: Create Visualizations



## Dashboard Report Overview

Explore a preview of our Zomato Power BI dashboard, offering key analytical insights into sales performance, customer trends, and business growth.

###

#### Intro Page: 
The navigation hub of the Zomato Analysis Power BI Dashboard. This page provides an overview of the dashboard’s purpose, highlighting key insights and ensuring a seamless user experience. It introduces users to different sections and helps them navigate through sales, marketing, and summary insights effectively.

![Image](https://github.com/user-attachments/assets/03ea149d-bc0d-4a4b-ba8f-5a676e328a95)

###

#### Sales & Revenue Analysis Page: 
A deep dive into restaurant sales performance across different time periods, cuisines, and locations. This page helps restaurant owners track revenue trends, identify high-performing categories, and optimize pricing strategies. It includes key metrics such as total sales, revenue, and sales distribution across various food categories, cities, and customer preferences.

![Image](https://github.com/user-attachments/assets/c1f28646-d063-4c51-a71a-33e54c61554e)

###

#### Marketing & Performance Analysis Page: 
Focuses on customer segmentation, marketing impact, and overall performance evaluation. It helps businesses understand how different factors influence sales and customer retention. Insights include revenue trends by age and occupation, customer segmentation based on income levels, and sales influenced by customer ratings and family size.

![Image](https://github.com/user-attachments/assets/404073f3-2791-463a-b2ee-5f6bba745464)
###

#### Summary Page: 
A comprehensive overview of Zomato's performance from 2020 to 2023, covering revenue trends, customer behavior, and operational efficiency. This page consolidates key insights to support data-driven decision-making and provides actionable recommendations for optimizing sales and marketing strategies.

![Image](https://github.com/user-attachments/assets/21b188ed-bc68-4fe3-9490-9fc565879225)
