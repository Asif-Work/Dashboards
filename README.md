# Healthcare Data Analysis-Dashboard

### Dashboard Link : [https://app.powerbi.com/groups/me/reports/384d017e-e935-44dc-9e7d-1626c1a36de1/ReportSection](https://app.powerbi.com/view?r=eyJrIjoiNjg0MGRlZTgtOWZhZC00YTUxLTk3MGQtNWQ1OTI3Y2E5NGQyIiwidCI6Ijk4YzJkMGYzLWRhYjctNDg1MS04MTA5LWJlYmUwNzdiYjU4NyIsImMiOjEwfQ%3D%3D)

## Introduction

In this project I developed an interactive Power BI dashboard for showing a particular data analysis on patient waiting list in a hospital. I used a publicly available healthcare data about the patient waiting list. The main goal of this project was to compare the specific metrics between inpatient and outpatient waiting lists based on other different categories.

## Data Overview
1. Inpatient: Treatment where a patient stays overnight in a hospital or medical facility.
2. Outpatient: Treatment that allows the patient to return home the same day without an overnight stay in a medical facility.

## Goals:
 1. Track status of current patient waiting lists(dynamic) and compare it to the previous year data.
 2. Analyze historical monthly trend of waiting lists in inpatient and outpatient categories.
 3. Detailed specialty level and age profile analysis.

## Data Scope:
The time frame of my data was of four years: 2018-2021

## Selected Metrics:
 For this analysis the metrics that I selected were:
 1. The average of waiting lists
 2. The median of waiting lists (as data might contain outliers)
 3. Current total waiting lists.

## Selected Visuals:
 I tried to portray the analysis into a two-page visualization. The first page shows the summary of the data analysis, and the second page depicts the granular perspective with a matrix.
 
### Steps followed 
Data Collection:
- Step 1 : Set all the dataset for inpatients and outpatients in csv format into 2 separate folders
- Step 2 : Connect the folders directory to Power BI

Transformation & Modeling:
- Step 3 : Check the data type of each column and make sure they are in correct format.
- Step 4 : Add "Case_Type" column to Outpatient table
- Step 5 : Append the tables as new table All_Data.
- Step 4 : Hide the inpatient and outpatient table in the modeling section.
- Step 6 : Make a custom mapping table for the specialty column as it has a large scale of categories and connect the csv file to Power BI.
- Step 7 : Connect the mapping table to the All data table.

Visualization Blueprint:
- Step 8 : Create the draft of the dashboard.
- Step 9 : Make 2 background layouts in the MS PowerPoint.

Layout & Design Workflow:
- Step 10 : Make new measure using DAX:
  ![image](https://github.com/user-attachments/assets/e15e5673-114d-4818-86d0-e036d158b836)

- Step 11 : DAX: ![image](https://github.com/user-attachments/assets/fca5293e-cde0-48e7-b078-02826613f432)

- Step 12 : Make a dummy table named CM with column: Average, Median.
- Step 13 : Using slicer make two buttons for Average and Median.
- Step 14 : Make the buttons functioning with anew measure containing DAX:![image](https://github.com/user-attachments/assets/ce7aa227-3738-4c57-aade-9521580fddf9)
- Step 15 : Link a donut chart with Avg/Median toggle.
- Step 16 : Put bar chart containing Time Bands as X axis, Avg/Median toggle as Y axis, and age_profile as legends.
- Step 17 : Transform the data once more to remove the duplicates and blank values from the age_profile column.
- Step 18 : Multi row card for Specialty_Name and Avg/Median toggle. Apply filter for top 5 value.
- Step 19 : Add line chart for Archive_Date as X axis, Sum of Toal as Y axis, and Case Type as legends. Filter the data only for Inpatient and Day Case.
- step 20 : Copy and Paste the line chart and filter it for only outpatient.
- Step 21 : Add Specialty and Case Type drop downs and a slicer for the archive date.
- Step 22 : Name this page as Summary.
- Step 23 : Add a new page for Granular analysis keeping the dropdwons and slicer.
- Step 24 : Add two more dropdowns for Age Profile and Time Band
- Step 25 : Add a Matrix view where rows are Archive Date, Specialty Name, Age Profile, and Time Bands and column is case type with legends having Sum of Total.
- Step 26 : Prepare a better tooltip for the line charts of Inpatient and Outpatient.
- 

## Snaps
Snap of the Appended table:

![All_Data](https://github.com/user-attachments/assets/6398e52c-53c9-43c9-886c-29d88b3bdefd)

Snap of the Data Model:

![Modeling](https://github.com/user-attachments/assets/267d1102-d8fd-4c24-b770-9c26e361ad0a)

Snap of all the tables and measures:

![image](https://github.com/user-attachments/assets/ed67a35f-4d39-4f57-88b6-a49ed8718c11)

Snap of the Summary Page:

![Slide2](https://github.com/user-attachments/assets/6bacf7cc-03fc-496f-9e43-2b6d60e29f14)

Snap of the Granular Page:

![Slide3](https://github.com/user-attachments/assets/5acae2dc-a317-43f3-9e14-a1c4dbe15691)
