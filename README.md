<h1 align="center" style="color:#8B008B; font-size:45px;">📊 Healthcare Data Analytics Dashboard</h1>
<h2 style="color:#C71585;">🌟 Project Overview</h2>

This project showcases a complete Healthcare Data Analytics Dashboard built using Microsoft Excel, covering:

Data Cleaning

Data Transformation

Pivot Tables

Quick Analysis

Dashboard Creation

All datasets were merged into a unified sheet using XLOOKUP + Data Model.

📅 Date: 25 Nov 2025
👩‍💻 Author: Indhira S — Aspiring Data Analyst

<h2 style="color:#C71585;">📌 Dashboard Preview</h2>

https://github.com/Indhiras6423/Excel-AI-Powered-Healthcare-Data-Insights-and-Dashboarding/blob/main/Screenshot%202025-11-24%20083504.png?raw=true

<h2 style="color:#C71585;">🗃️ Dataset Fields</h2>
Field	Description
🆔 Customer ID	Unique identifier
👤 First Name	Patient’s name
⚖️ BMI	Body Mass Index
🩸 HBA1C	Glucose level indicator
❤️ Heart Issues	Yes/No
🏥 Any Transplants	Yes/No
🎗️ Cancer History	Yes/No
🔪 Major Surgeries	Number of surgeries
🚬 Smoker	Yes/No
⚖️ Weight Status	Underweight / Normal / Overweight / Obesity
🩺 Diabetes Status	Diabetic / Pre-Diabetic / Normal
🎂 Date of Birth	Cleaned + formatted
💵 Charges	Hospitalization cost
🏥 Hospital Tier	Tier-1 / Tier-2 / Tier-3
🌆 City Tier	Tier classification
🆔 State ID	State-level identifier
🎯 Age	Calculated age (as of 8 June 2023)
<h2 style="color:#C71585;">🧹 Data Cleaning Steps</h2>

✔️ Replaced “?” missing values
✔️ Filled missing Month → September
✔️ Filled missing Year → rounded average
✔️ Filled missing Smoker, City Tier, Hospital Tier → MODE()
✔️ Missing State ID → replaced with “Unknown”
✔️ Converted Major Surgeries to numeric
✔️ Split Name → Title / First / Last
✔️ Created DOB from Year + Month + Date
✔️ Created Age using TODAY() logic
✔️ Formatted Charges → Currency ($)

<h2 style="color:#C71585;">🧮 Key Formulas Used</h2>
🔧 Cleaning & Transformation
=IF(cell="?", "", cell)
=TEXT(DATE(Year, Month, Date),"DD-MMM-YYYY")
=INT((DATE(2023,6,8)-DOB)/365)

🔍 Lookup & Merge
=XLOOKUP(CustomerID, Table1[ID], Table1[Column])

📊 BMI Category (Weight Status)
=IF(BMI<18.5,"Underweight",
IF(BMI<25,"Normal Weight",
IF(BMI<30,"Overweight","Obesity")))

<h2 style="color:#C71585;">📊 Dashboard Insights</h2>

🔸 Smokers vs Non-Smokers — Cancer History
Smokers show higher cancer incidence → higher lifestyle risk.

🔸 Charges by Weight Status
Obese patients → highest total healthcare spending.

🔸 Hospital Tier Analysis
Tier-3 hospitals → highest average hospitalization charges.

🔸 Diabetes & HBA1C
Higher HBA1C strongly correlates with diabetic patients.

🔸 Weight Status Distribution
Majority fall under Obesity and Overweight groups.

<h2 style="color:#C71585;">🛠️ Tools Used</h2>

Microsoft Excel

Pivot Tables

Pivot Charts (Pie, Doughnut, Column, Bar)

Quick Analysis

Slicers

Data Model + XLOOKUP

<h2 style="color:#C71585;">🏁 Conclusion</h2>

This Healthcare Dashboard demonstrates strong Excel analytics skills, showcasing end-to-end workflow from data cleaning to business insights for medical decision-making.

<h2 style="color:#C71585;">💼 Connect With Me</h2>

🔗 LinkedIn: www.linkedin.com/in/indhira4623
