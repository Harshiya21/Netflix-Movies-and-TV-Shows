# Netflix-Movies-and-TV-Shows
# Netflix Data Analysis Dashboard (Power BI)

## Project Overview
This project analyzes Netflix content to identify trends in genres, ratings, release years, and audience engagement.  
Built entirely using **Power BI**, **Power Query**, and **DAX**.

## Tools & Techniques
- **Power BI** for visualization & dashboard creation  
- **Power Query** for data cleaning and transformation  
- **DAX** for calculated columns and measures

## Data Cleaning (Power Query)
- Removed duplicates and null values
- Split combined columns (e.g., Director/Actor lists)
- Transformed date and duration fields
- Filtered invalid or incomplete records

## DAX Measures
Some key measures used:
```DAX
Total_Titles = COUNTROWS(Netflix)
Average_Duration = AVERAGE(Netflix[Duration])
Top_Genres = CALCULATE(COUNTROWS(Netflix), ALLEXCEPT(Netflix, Netflix[Genre]))
