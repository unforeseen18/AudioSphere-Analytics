# AudioSphere-Analytics

## Overview

AudioSphere-Analytics is a data analytics project developed using PostgreSQL and PgAdmin4 to analyze the business performance of an online music store. The project focuses on extracting meaningful insights from music sales data using SQL queries and relational database concepts.

The analysis helps identify customer purchasing behavior, top-performing artists, popular music genres, revenue trends, and regional sales performance to support data-driven business decisions.

---

## Project Objectives

* Analyze customer purchasing patterns
* Identify top-selling artists, albums, and tracks
* Understand music genre popularity
* Evaluate country-wise revenue generation
* Perform business intelligence analysis using SQL

---

## Technologies Used

* PostgreSQL
* PgAdmin4
* SQL
* CSV Dataset

---

## Database Setup

1. Install PostgreSQL and PgAdmin4
2. Create a new database
3. Import the provided CSV dataset files
4. Create tables using the schema diagram
5. Execute the SQL queries from the analysis file

---

## Database Schema

The project uses a relational database schema consisting of multiple interconnected tables including:

* Customer
* Invoice
* InvoiceLine
* Track
* Album
* Artist
* Genre
* Playlist
* Employee

These tables are connected using primary and foreign key relationships to support advanced SQL analysis.

---

## Key Business Questions Solved

* Which music genre generates the highest sales?
* Who are the top-performing artists?
* Which songs are purchased the most?
* Which countries contribute the highest revenue?
* What are the customer purchasing trends?
* Which albums and playlists are most popular?

---

## Project Insights

* Rock emerged as one of the most purchased music genres
* Certain artists generated significantly higher revenue compared to others
* The United States showed the highest customer purchase activity
* Customer buying patterns helped identify popular music preferences

---

## Features

* Advanced SQL query analysis
* Relational database design
* Business performance evaluation
* Customer behavior analysis
* Revenue and sales insights
* Data-driven reporting

---

## Installation Requirements

* PostgreSQL
* PgAdmin4

---

## Repository Structure

AudioSphere-Analytics/
│
├── dataset/
├── analysis.sql
├── schema.sql
├── README.md
└── assets/

---

## Future Enhancements

* Power BI dashboard integration
* Interactive sales visualization
* Python-based analytics automation
* Music recommendation analysis
* Real-time reporting dashboard

---

## Author

Prajaktaa Chhetri

GitHub Repository:
[https://github.com/unforeseen18/AudioSphere-Analytics](https://github.com/unforeseen18/AudioSphere-Analytics)

---

--------------------------------------------------

## Python and Power BI Integration

### Python Integration

The project can be integrated with Python to automate data analysis, generate reports, and perform advanced analytics on music store data.

### Step 1: Install Required Python Libraries

Install the following libraries using pip:

pip install pandas psycopg2 matplotlib

### Step 2: Connect PostgreSQL Database with Python

Create a Python file and establish a database connection.

Example:

import psycopg2
import pandas as pd

conn = psycopg2.connect(
    host="localhost",
    database="music_store",
    user="postgres",
    password="your_password"
)

query = "SELECT * FROM invoice"
df = pd.read_sql(query, conn)

print(df.head())

### Step 3: Perform Data Analysis using Python

Python can be used for:

- Customer purchase analysis
- Revenue trend analysis
- Genre popularity analysis
- Artist performance analysis
- Automated report generation

### Step 4: Export Processed Data

Export analyzed data into CSV format for reporting and dashboard creation.

Example:

df.to_csv("sales_report.csv", index=False)

--------------------------------------------------

## Power BI Integration

Power BI can be integrated with PostgreSQL to create interactive dashboards and visual reports.

### Step 1: Install Power BI Desktop

Download and install Power BI Desktop from Microsoft's official website.

### Step 2: Connect PostgreSQL Database to Power BI

1. Open Power BI Desktop
2. Click on Get Data
3. Select PostgreSQL Database
4. Enter:
   - Server Name
   - Database Name
5. Connect using PostgreSQL credentials

### Step 3: Import Tables

Import required tables such as:

- Customer
- Invoice
- InvoiceLine
- Track
- Artist
- Genre
- Album

### Step 4: Create Interactive Dashboards

Build dashboards for:

- Sales Performance
- Genre Popularity
- Top Artists
- Country-wise Revenue
- Customer Purchasing Trends

### Step 5: Add Visualizations

Recommended visualizations include:

- Bar Charts
- Pie Charts
- Line Graphs
- KPI Cards
- Maps
- Slicers and Filters

### Step 6: Generate Business Insights

Power BI dashboards help generate visual business insights for decision-making and performance evaluation.

--------------------------------------------------

## Integrated Project Workflow

PostgreSQL Database
        ↓
SQL Query Analysis
        ↓
Python Data Processing
        ↓
CSV/Data Export
        ↓
Power BI Dashboard Visualization
        ↓
Business Insights and Reporting

--------------------------------------------------

## Benefits of Python and Power BI Integration

- Automated analytics workflow
- Interactive business dashboards
- Better data visualization
- Advanced business intelligence reporting
- Improved decision-making using analytics
- Enhanced project scalability and professionalism

--------------------------------------------------
## License

This project is intended for educational and academic purposes. The dataset can be used for practicing SQL queries, database management, and analytics concepts.
