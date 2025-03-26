# SQL-Data_Cleaning_Project

🔍 Project Overview

This project focuses on data cleaning using MySQL to preprocess a dataset containing layoffs data. The dataset includes information about company layoffs, industries, locations, and other relevant details. The goal is to ensure data consistency, accuracy, and usability by performing essential cleaning tasks.

Data Cleaning Steps

1. Removing Duplicates

Identified duplicate rows based on company name, location, industry, total layoffs, percentage layoffs, date, stage, country, and funds raised.

Used ROW_NUMBER() to mark duplicate entries.

Deleted duplicate rows from the dataset.

2. Standardizing Data

Standardized industry names (e.g., changing different variations of "Crypto" to a single format).

Standardized country names to avoid inconsistencies (e.g., "United States " → "United States").

3. Handling Null and Blank Values

Identified and removed rows where both total_laid_off and percentage_laid_off were NULL.

Replaced blank industry values by referencing other rows with the same company name.

Ensured there were no empty strings in critical columns.

4. Removing Unnecessary Columns

Dropped the row_num column, which was used for duplicate detection but is no longer needed.


 📌 SQL Queries Used

The project includes SQL queries for:

Creating staging tables to work on a copy of the original dataset.

Identifying and deleting duplicate records using ROW_NUMBER().

Standardizing values to maintain uniformity in data.

Handling missing values by either filling them with reference data or removing unnecessary records.

Formatting date fields to ensure consistency.

Dropping unnecessary columns to streamline the dataset.


📌 Technologies Used

MySQL for database management and data cleaning.

SQL Queries for transformations and modifications.

GitHub for version control and project documentation.
