# Crowdfunding ETL

![Crowdfunding ETL](https://github.com/claytonmknight/Crowdfunding_ETL/assets/148498483/755282da-ee89-440e-b903-4dc13de8e7f9)

## Introduction
Crowdfunding ETL is a project focusing on Extract, Transform, Load (ETL) processes using Python, Pandas, and various data manipulation techniques. The project aims to extract data from Excel files, transform it into structured formats, and load it into a PostgreSQL database. This README provides an overview of the project structure, objectives, and steps involved in the ETL process.

## Contributors
- Marsha Cole
- Clayton Knight

## Project Overview
The project involves the following key components:

1. **Data Extraction and Transformation**: Extracting data from Excel files (`crowdfunding.xlsx` and `contacts.xlsx`) and transforming it into structured CSV files.
2. **Database Creation**: Designing and creating a PostgreSQL database schema based on the transformed data.
3. **ETL Pipeline**: Developing Python scripts to execute the ETL process, including loading data into the database.
4. **Documentation**: Providing detailed documentation, including project outline, file descriptions, and database schema.

## Files Included
- **[Crowdfunding_db_schema.sql](https://github.com/claytonmknight/Crowdfunding_ETL/blob/main/Crowdfunding_db_schema.sql)**: PostgreSQL database schema script.
- **[ETL_Mini_Project_MCole_CKnight.ipynb](https://github.com/claytonmknight/Crowdfunding_ETL/blob/main/ETL_Mini_Project_MCole_CKnight.ipynb)**: Jupyter Notebook containing Python code for data extraction, transformation, and loading.
- **[QuickDBD-Crowdfunding ELT.png](https://github.com/claytonmknight/Crowdfunding_ETL/blob/main/QuickDBD-Crowdfunding%20ETL.png)**: Entity-Relationship Diagram (ERD) representing the database schema.
- **Screenshots**: Screenshots of sample data and tables.
- **[Resources](https://github.com/claytonmknight/Crowdfunding_ETL/tree/main/Resources)**: Folder containing source Excel files and generated CSV files.

## Project Outline
The project is divided into the following subsections:

1. **Create the Category and Subcategory DataFrames**: Extracting and transforming data from `crowdfunding.xlsx` to create category and subcategory CSV files.
2. **Create the Campaign DataFrame**: Extracting and transforming data from `crowdfunding.xlsx` to create a campaign CSV file.
3. **Create the Contacts DataFrame**: Extracting and transforming data from `contacts.xlsx` to create a contacts CSV file.
4. **Create the Crowdfunding Database**: Designing the database schema, creating tables, and importing CSV data into the PostgreSQL database.

## Usage
To execute the ETL process, follow these steps:
1. Run the Jupyter Notebook `ETL_Mini_Project_MCole_CKnight.ipynb`.
2. Ensure all dependencies are installed (`pandas`, `sqlalchemy`, etc.).
3. Follow the instructions provided in the notebook to execute each step of the ETL process.
4. Verify the database creation and data import by querying the PostgreSQL database.

## Database Schema
The database schema is represented in the ERD below:

![QuickDBD-Crowdfunding ETL](https://github.com/claytonmknight/Crowdfunding_ETL/assets/153461955/1eb5fe61-326e-463e-bbcd-3ff4f9425267)

The schema is defined in the script `Crowdfunding_db_schema.sql`.

## Screenshots
Sample screenshots of the created database tables:

- **Contacts Table**
  
      ![Screenshot Contacts](https://github.com/claytonmknight/Crowdfunding_ETL/assets/153461955/98573ab9-a1d3-4ce4-a931-7d3e45cc4682)

- **Category Table**
  
      ![Screenshot Category](https://github.com/claytonmknight/Crowdfunding_ETL/assets/153461955/c8653ec5-bc93-4dab-aa3d-f90822cc412d)

- **Subcategory Table**
  
      ![Screenshot Subcategory](https://github.com/claytonmknight/Crowdfunding_ETL/assets/153461955/65d67b80-88f9-488e-990e-4d2fd8ff343f)

- **Campaign Table**
  
      ![Screenshot Campaign](https://github.com/claytonmknight/Crowdfunding_ETL/assets/153461955/786551dd-f232-4c4a-82cd-ee2c66bd1d0e)

## Conclusion
The Crowdfunding ETL project demonstrates the process of extracting, transforming, and loading data from Excel files into a PostgreSQL database. The provided scripts and documentation serve as a guide for understanding and replicating the ETL process for similar datasets.
