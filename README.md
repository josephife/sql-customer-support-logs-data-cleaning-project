# sql-customer-support-logs-data-cleaning-project
A SQL-based data cleaning project on messy customer support logs. Tasks included handling missing values, standardizing text and dates, removing duplicates, and preparing the dataset for analysis.

 Customer Support Logs – Data Cleaning Project
Author: Joseph Ifechukwu
Portfolio Site: Data by Joseph Ifechukwu
Focus: Data Cleaning | SQL (MySQL) | Data Preparation for Analysis

 Project Overview
This project involved cleaning and standardizing a raw dataset containing customer support logs. The dataset was originally messy, with formatting issues, missing values, duplicates, and inconsistent data types, making it unfit for analysis.

Using MySQL, I performed several data cleaning tasks to transform it into a well-structured dataset ready for further analysis and reporting.

 Tools Used
SQL (MySQL Workbench)

WordPress (for documentation)

 Dataset Summary
Source: Sample dataset for practicing data cleaning in SQL

Size: ~1000 rows

Key Columns:

customer_name

customer_email

ticket_id

issue_category

issue_description

created_at

resolved_at

status

assigned_agent

 Cleaning Steps
1.  Database Setup
Created a new database in MySQL.

Imported the raw dataset via MySQL Workbench.

Created a backup of the raw data for reference.

2.  Handling Missing Values
Identified NULL values across all columns.

Replaced missing customer names and statuses with 'Unknown'.

Removed leading/trailing spaces using TRIM().

3. Text Standardization
Converted all text to lowercase using LOWER().

Removed unwanted symbols using REPLACE() and REGEXP_REPLACE() (e.g., !, #, @).

Corrected wrongly formatted emails using pattern matching and SQL updates.

4. Date Formatting
Standardized inconsistent date formats (e.g., April 2, 2023, 2-04-23) to YYYY-MM-DD using STR_TO_DATE() and DATE_FORMAT().

5.  Duplicate Handling & Keys
Used ROW_NUMBER() to identify and remove duplicate rows.

Ensured ticket_id uniqueness; added a new primary key column if needed.

6.  Data Types & Column Names
Renamed columns for clarity (e.g., created_at → date_created).

Changed data types:

Converted text to DATE or INT as needed.

 Results
The cleaned dataset is now:

Free of missing or invalid email addresses.

Using a consistent date format.

Standardized in text values and formatting.

Structured with clear, analysis-ready columns and types.



![Raw Dataset] ![Screenshot (269)](https://github.com/user-attachments/assets/e1effcff-16d0-4a37-9d0f-830a129e336e)

![Cleaned Dataset]![Screenshot (268)](https://github.com/user-attachments/assets/7b5d73cb-516d-4970-8e99-f70573f0c84e)

🔗 Project Motto
"Transforming Data into Insights and Visual Stories"
  Data by Joseph Ifechukwu

