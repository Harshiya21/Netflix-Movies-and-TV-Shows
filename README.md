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

## Dashboard Overview   
<img width="1479" height="827" alt="image" src="https://github.com/user-attachments/assets/fc1b8243-a74a-4f15-9050-e2dbf2da65bb" />

## Total Movies and Tv Shows by Release Year
<img width="1770" height="860" alt="image" src="https://github.com/user-attachments/assets/3c913868-13cd-4792-b767-5971224df80b" />

## Ratings by Total Titles
<img width="1799" height="820" alt="image" src="https://github.com/user-attachments/assets/71d8dbd5-d019-41db-9c4e-6e3128508f15" />

## Insights
- International Movies and Dramas have grown over the years

- Movies and TV Shows increased significantly between 2015–2020

- TV-MA is the most common rating

- The U.S. and India produce the most content

- Drama and Comedy are the most popular genres

- The majority of Netflix titles are Movies

## DAX Measures
Some key measures used:
```DAX
Total_Titles = COUNTROWS(Netflix)
Average_Duration = AVERAGE(Netflix[Duration])
Total Shows = CALCULATE(DISTINCTCOUNT('category mapping'[show_id]))
