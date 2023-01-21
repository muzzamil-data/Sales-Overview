# Sales-Overview


<img width="765" alt="Salesoverview" src="https://user-images.githubusercontent.com/123259830/213881604-637727b5-3ab1-4c78-91b8-dbc55dd6ca04.png">

# Product details
<img width="757" alt="Product details" src="https://user-images.githubusercontent.com/123259830/213881830-0a4d38ab-0205-45b7-8d52-d5344fefcca9.png">

# Customer details
<img width="758" alt="Customer details" src="https://user-images.githubusercontent.com/123259830/213881867-b037393e-a351-4dcf-b080-88b9bbf8239b.png">

# SQL Statement 
<![sql_statement](https://user-images.githubusercontent.com/123259830/213882189-7fb4f4b4-6111-4bbc-bd30-32225b8cd4bc.png)

# Business Request & User Stories
The business request for this data analyst project was an executive sales report for sales managers. Based on the request that was made from the business we following user stories were defined to fulfill delivery and ensure that acceptance criteria’s were maintained throughout the project.

<img width="440" alt="Business demand overview" src="https://user-images.githubusercontent.com/123259830/213882478-5e37b2e6-9aac-49a8-bc69-aa12bb829823.png">

# Data Cleansing & Transformation (SQL)
To create the necessary data model for doing analysis and fulfilling the business needs defined in the user stories the following tables were extracted using SQL.

One data source (sales budgets) were provided in Excel format and were connected in the data model in a later step of the process.

Below are the SQL statements for cleansing and transforming necessary data.

# DIM_Calendar:
# -- Cleansed DIM_Date Table --
`SELECT 
  [DateKey], 
  [FullDateAlternateKey] AS Date, 
  --[DayNumberOfWeek], 
  [EnglishDayNameOfWeek] AS Day, 
  --[SpanishDayNameOfWeek], 
  --[FrenchDayNameOfWeek], 
  --[DayNumberOfMonth], 
  --[DayNumberOfYear], 
  --[WeekNumberOfYear],
  [EnglishMonthName] AS Month, 
  Left([EnglishMonthName], 3) AS MonthShort,   -- Useful for front end date navigation and front end graphs.
  --[SpanishMonthName], 
  --[FrenchMonthName], 
  [MonthNumberOfYear] AS MonthNo, 
  [CalendarQuarter] AS Quarter, 
  [CalendarYear] AS Year --[CalendarSemester], 
  --[FiscalQuarter], 
  --[FiscalYear], 
  --[FiscalSemester] 
FROM 
 [AdventureWorksDW2019].[dbo].[DimDate]
WHERE 
  CalendarYear >= 2019`



