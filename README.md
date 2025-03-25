AtliQ Grands Hospitality Analysis
This repository contains a Power BI project aimed at providing valuable insights to the Revenue Management Team at AtliQ Grands, a chain of five-star hotels across India. This project showcases the data analysis process, including data cleaning, data modeling, and creating interactive dashboards to help AtliQ Grands regain their market share and increase revenue in the luxury/business hotels category.

Table of Contents
Project Overview
Dataset
Data Preparation & Cleaning
Data Modeling & DAX Measures
Dashboard
Key Insights
How to Use
Technologies Used


1. Project Overview
Business Context: AtliQ Grands has been experiencing declining market share and revenue due to increased competition and ineffective decision-making.

Goal: Provide actionable insights to the revenue management team using historical data, helping them make data-driven decisions to improve occupancy, increase revenue, and optimize overall performance.

Scope:
Create metrics (KPIs) as specified in the requirements.
Develop an interactive dashboard following the given mock-up.
Provide additional insights beyond the initial mock-up and metrics list.

2. Dataset
The project uses sample/historical data related to AtliQ Grands’ hotel operations. Key tables include:
fact_bookings
fact_aggregated_bookings
dim_date
dim_hotels
dim_rooms
key_measures

The data contains information about bookings, revenue, room categories, hotels, and time dimensions.

3. Data Preparation & Cleaning
Data Source: Imported from provided CSV/Excel files into Power BI.
Power Query:
Removed unnecessary columns.
Fixed data types (e.g., date fields, numeric fields).
Handled missing or null values.
Created new columns where necessary for better reporting (e.g., month names, year columns, etc.).
Data Validation: Verified row counts and spot-checked random entries to ensure data integrity.

4. Data Modeling & DAX Measures
Data Modeling
Established one-to-many relationships among dimension and fact tables.
Ensured the star schema approach, linking fact tables (e.g., fact_bookings) to dimension tables (dim_hotels, dim_date, dim_rooms).
DAX Measures
Created key measures such as:
Total Revenue: SUM(fact_bookings[revenue])
ADR (Average Daily Rate): DIVIDE([Total Revenue], [Number of Room Nights])
Occupancy %: DIVIDE([Occupied Rooms], [Available Rooms])
RevPAR (Revenue per Available Room): DIVIDE([Total Revenue], [Available Rooms])
Avg Rating: AVERAGE(fact_bookings[rating])
Realisation %: DIVIDE([Successful Bookings], [Total Bookings])
(Note: Names/formulas may vary depending on how they were actually implemented.)

5. Dashboard
An interactive Power BI dashboard was designed based on stakeholder requirements and a provided mock-up. The dashboard includes:
High-Level KPIs:
Total Revenue
RevPAR
Occupancy %
ADR
Average Rating
Filters/Slicers:
Filter by City
Filter by Room
Date Range Filters

Visualizations:
Pie/Donut Charts: Occupancy by Category
Line/Area Charts: Weekly trends of ADR, RevPAR, Occupancy, and Revenue
Bar Charts: Realisation % and ADR by Booking Platform
Tables: Detailed breakdown of key metrics by property name, city, and room category

6. Key Insights
Some of the actionable insights drawn from the dashboard:
Revenue Distribution: Identified top-performing cities and hotels contributing the highest revenue.
Occupancy Trends: Pinpointed peak occupancy months/weeks and periods of low occupancy.
ADR & RevPAR Analysis: Revealed how ADR and RevPAR vary by room category (Luxury, Business) and seasonality.
Booking Platform Performance: Highlighted which booking platforms yield the highest realisation and revenue, guiding marketing focus.
Cancellation & Refund Rates: Exposed patterns in cancellations, aiding the team in formulating better policies to reduce cancellations.
Rating Analysis: Correlated ratings with occupancy and revenue to see how customer satisfaction impacts profitability.

7. How to Use
Clone or Download this repository.
Open the Power BI file (.pbix) in Microsoft Power BI Desktop.
Ensure you have the correct data sources (CSV/Excel files). If the dataset paths differ, update them in Power Query
Refresh the data in Power BI.
Explore the dashboard using slicers/filters to generate insights tailored to specific cities, room categories, and time periods.

8. Technologies Used
Power BI: Data ingestion, modeling, visualization
Power Query: Data cleaning and transformation
DAX (Data Analysis Expressions): Calculations and measures


END OF FILE!
