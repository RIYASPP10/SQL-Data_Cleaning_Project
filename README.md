# SQL-Data_Cleaning_Project

Project Overview

This project focuses on data cleaning using MySQL to preprocess a dataset containing layoffs data. The dataset includes information about company layoffs, industries, locations, and other relevant details. The goal is to ensure data consistency, accuracy, and usability by performing essential cleaning tasks.

Data Cleaning Steps

1. Removing Duplicates

Identified duplicate rows based on company name, location, industry, total layoffs, percentage layoffs, date, stage, country, and funds raised.

Used ROW_NUMBER() to mark duplicate entries.

Deleted duplicate rows from the dataset.
