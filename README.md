# Sales-Overview


# Business Request & User Stories
The business request for this data analyst project was an executive sales report for sales managers. Based on the request that was made from the business we following user stories were defined to fulfill delivery and ensure that acceptance criteria’s were maintained throughout the project.

<img width="440" alt="Business demand overview" src="https://user-images.githubusercontent.com/123259830/213882478-5e37b2e6-9aac-49a8-bc69-aa12bb829823.png">

# Data Model
Below is a screenshot of the data model after cleansed and prepared tables were read into Power BI.

This data model also shows how FACT_Budget hsa been connected to FACT_InternetSales and other necessary DIM tables.

<img width="764" alt="DATAMODEL" src="https://user-images.githubusercontent.com/123259830/213883378-b248cb58-3759-4576-856d-b6bab6772a89.png">

# Sales Management Dashboard
The finished sales management dashboard with one page with works as a dashboard and overview, with two other pages focused on combining tables for necessary details and visualizations to show sales over time, per customers and per products.

<img width="765" alt="Salesoverview" src="https://user-images.githubusercontent.com/123259830/213881604-637727b5-3ab1-4c78-91b8-dbc55dd6ca04.png">

# Product details
<img width="757" alt="Product details" src="https://user-images.githubusercontent.com/123259830/213881830-0a4d38ab-0205-45b7-8d52-d5344fefcca9.png">

# Customer details
<img width="758" alt="Customer details" src="https://user-images.githubusercontent.com/123259830/213881867-b037393e-a351-4dcf-b080-88b9bbf8239b.png">

# Data Cleansing & Transformation (SQL)
To create the necessary data model for doing analysis and fulfilling the business needs defined in the user stories the following tables were extracted using SQL.

One data source (sales budgets) were provided in Excel format and were connected in the data model in a later step of the process.

Below are the SQL statements for cleansing and transforming necessary data.

# DIM_Calendar:
<img width="737" alt="CLEANSED DIM_Date Table" src="https://user-images.githubusercontent.com/123259830/213883175-5db989f8-223f-421a-8170-c51443e365b6.png">

# DIM_Customers:
<img width="368" alt="Cleansed DIM_Customers Table " src="https://user-images.githubusercontent.com/123259830/213883209-a044f95d-b933-4516-ab2a-6221ddfa8102.png">

# DIM_Products:
<img width="410" alt="Cleansed DIM_Products Table " src="https://user-images.githubusercontent.com/123259830/213883239-ccedcc88-f61c-4fef-998c-0cfac1a4b0fc.png">

# FACT_InternetSales:
<img width="470" alt="Cleansed FACT_InternetSales Table" src="https://user-images.githubusercontent.com/123259830/213883269-1c8bae1c-b3b6-42f0-8410-913dde584538.png">












