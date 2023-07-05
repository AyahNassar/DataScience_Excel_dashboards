# Bike Sales Dashboard in Excel

## Overview
This README file outlines the process we've used to analyze and visualize bike sales data in an interactive Excel dashboard. Our data analysis journey includes data cleaning, feature engineering, and creating pivot tables for interactive visual analytics.

## Data Description
The dataset comprises 13 columns and 1001 rows, representing 1000 customers with their respective demographic and sales information. The columns include:

1. ID
2. Marital Status (Single/Married)
3. Gender (Female/Male)
4. Income
5. Children
6. Education (Bachelors, Masters, College)
7. Occupation (Skilled manual, Professional, Clerical, Manual, Management)
8. Home Owner (Yes/No)
9. Cars 
10. Commute Distance (0-1, 2-5, 5-10, More than 10 miles)
11. Region (Europe, North America, Pacific)
12. Age
13. Bike Purchase (Yes/No)

## Data Cleaning
Before we could analyze the data, we had to ensure it was clean and free of inaccuracies. Here are the key Excel techniques we employed:

* **Find & Replace (Ctrl+H):** Used to replace category codes with their full meaning (e.g., 'M' with 'Married' and 'S' with 'Single' in the Marital Status column).

* **Remove Duplicates:** Excel's built-in function was used to ensure all customers' data is unique.

* **Currency Formatting:** We specified the currency for the 'Income' column to provide clarity on income values.

## Feature Engineering
We leveraged Excel's `IF` function to create a new column, 'Age Brackets,' categorizing customers into 'Adolescent', 'Middle Age', and 'Old'. Feature engineering is a critical step in data analysis, enhancing the understanding of data and improving model performance if predictive analysis is conducted later.

The formula used is `=IF(L2>54, "Old", IF(L2>=31, "Middle Age", IF(L2<31, "Adolescent", "Invalid")))`.

This new feature provides us with the ability to gain more granular insights about bike sales across different age groups.

## Data Analysis & Visualization
Three additional sheets were created to facilitate the analysis and visualization:

1. **Workspace:** This is a duplicate of the original data, allowing us to perform our operations without altering the original dataset.

2. **Pivot Tables & Visuals:** Multiple pivot tables were created to summarize and analyze the dataset, with corresponding visuals for each pivot table.

3. **Dashboard:** Here, we consolidated key insights into an interactive dashboard. We used Excel's built-in filter feature to enable filtering by Marital Status, Region, and Education.

## Importance of Data Exploration and Cleaning
Data exploration and cleaning are fundamental steps in any data analysis process. They ensure the quality and accuracy of the data, ultimately resulting in reliable insights. By thoroughly cleaning our data, we avoided skewed results, identified important trends, and built a robust, interactive dashboard to drive business decisions.

## Conclusion
With the clean dataset, a new feature for enriched insights, and a comprehensive dashboard, we can now analyze and understand the sales performance of bikes across different demographics and geographical locations, empowering strategic business decisions.
