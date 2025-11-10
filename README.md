# Netflix-Movies-and-TV-Shows
# Netflix Data Analysis Dashboard (Power BI)

## Project Overview
This project analyzes Netflix content to identify trends in genres, ratings, release years.
Built entirely using **Power BI**, **Power Query**, and **DAX**.

## Tools & Techniques
- **Power BI** for visualization & dashboard creation  
- **Power Query** for data cleaning and transformation  
- **DAX** for calculated columns and measures

## Data Cleaning (Power Query)
- Removed duplicates and null values
- Transformed date and duration fields
- Filtered invalid or incomplete records

## DAX Measures
Some key measures used:
```DAX
Total_Titles = COUNTROWS(Netflix)
Average_Duration = AVERAGE(Netflix[Duration])
Total Shows = CALCULATE(DISTINCTCOUNT('category mapping'[show_id]))

**## Key Insights**
- International Movies and Dramas have grown the most in total titles.
- Movies make up 70% of total content.
- Movies and TV shows have significantly increased between 2015 and 2020.
