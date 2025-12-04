🧪 Medical Report Dashboard — README
📌 Overview

This Power BI dashboard analyzes a medical dataset containing information on diagnosis types, gender, age groups, fever temperature, and diarrhea cases.
The goal of this report is to provide a clear visualization of health trends, fever case distribution, and gender-wise diagnosis patterns.

🔗 Data Connections / Data Sources

This dashboard is built using a single local Excel dataset.

1) Local Excel File

Source: medical_report.xlsx

Connection Type: Import

Tables/Columns Used:

Diagnosis

Gender

Age

Temperature_C

Diarrhea

Notes:

Data cleaned and transformed in Power Query

Null values removed

Data types corrected (Number/Text)

2) No external gateway

All transformations and calculations happen locally in Power BI Desktop.

🧩 Data Model (Small Details)

Fact Table: Fever/Diagnosis Records

Dimension Columns: Gender, Age, Diagnosis, Temperature_C, Diarrhea

Key Fields:

diagnosis

gender

age

temperature_c

diarrhea

Transformations Performed

Removed duplicates

Standardized temperature values

Created calculated fields for total fever cases

Grouped records for diagnosis and gender analysis

📏 Measures Used
Total Fever Cases = COUNTROWS(Data)
Count by Diagnosis = COUNT(Data[diagnosis])
Sum of Fever = SUM(Data[fever])
Gender Count = COUNT(Data[gender])


Additional implicit measures were generated automatically by Power BI for visual calculations.

📊 Visuals Included
1) Count by Diagnosis (Pie Chart)

Shows total patient distribution across:

Influenza

COVID-19

Dengue

Malaria

Pneumonia

2) Total Fever Cases (Card Visual)

Displays the overall fever case count: 3230

3) Sum of Fever by Temperature & Diarrhea (Stacked Column Chart)

Shows how fever cases vary across different temperature ranges

Breaks down fever counts based on diarrhea presence

4) Count of Gender by Diarrhea and Age (Line Chart)

Visualizes age-wise and gender-wise diarrhea distribution

5) Count of Diagnosis by Gender (Pie/Donut Chart)

Male vs Female diagnosis distribution:

Male: ~1.46K

Female: ~1.54K

6) Dashboard Header

Custom logo "Medical Report Database" placed at the top center.

🌱 Key Insights

Total fever cases analyzed: 3230

Female patients slightly outnumber male patients

COVID-19 and Influenza show the highest diagnosis counts

Some temperature ranges show higher diarrhea frequency

Age-wise diarrhea patterns reveal trends among child and teen groups

📁 How to Use

Download the .pbix file

Open in Power BI Desktop

No data gateway or fresh connection required

Publish to Power BI Service (optional)
