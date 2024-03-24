
<img width="1045" alt="image" src="https://github.com/claytonmknight/Crowdfunding_ETL/assets/148498483/755282da-ee89-440e-b903-4dc13de8e7f9">

# Crowdfunding_ETL
Project 2 - Group 4 
Contributors: Marsha Cole and Clayton Knight

# Introduction
In this Extract, Transform, Load (ETL) project, we built an ETL pipeline using Python, Pandas, and either Python dictionary methods or regular expressions to extract and transform the data. After transforming the data, we created four CSV files and used the CSV file data to create an ERD and a table schema. Finally, we uploaded the CSV file data into a Postgres database.

## Project Outline
This project was divided into the following subsections:

  * Create the Category and Subcategory DataFrames
  * Create the Campaign DataFrame
  * Create the Contacts DataFrame
  * Create the Crowdfunding Database

# Create the Category and Subcategory DataFrames
1. Extract and transform the `crowdfunding.xlsx` Excel data to create a category DataFrame that has the following columns:

   * A "category_id" column that has entries going sequentially from "cat1" to "catn", where n is the number of unique categories

   * A "category" column that contains only the category titles

2. Export the category DataFrame as `category.csv` and save it to your GitHub repository.

3. Extract and transform the `crowdfunding.xlsx` Excel data to create a subcategory DataFrame that has the following columns:

   * A "subcategory_id" column that has entries going sequentially from "subcat1" to "subcatn", where n is the number of unique subcategories

   * A "subcategory" column that contains only the subcategory titles

4. Export the subcategory DataFrame as subcategory.csv and save it to your GitHub repository.


# Create the Campaign DataFrame

1. Extract and transform the `crowdfunding.xlsx` Excel data to create a campaign DataFrame has the following columns:

   * The **"cf_id"** column
   
   * The **"contact_id"** column
   
   * The **"company_name"** column
   
   * The **"blurb"** column, renamed to ***"description"***
   
   * The **"goal"** column, converted to the float data type
   
   * The **"pledged"** column, converted to the float data type
   
   * The **"outcome"** column
   
   * The **"backers_count"** column
   
   * The **"country"** column
   
   * The **"currency"** column
   
   * The **"launched_at"** column, renamed to ***"launch_date"*** and with the UTC times converted to the datetime format
   
   * The **"deadline"** column, renamed to ***"end_date"*** and with the UTC times converted to the datetime format
   
   * The **"category_id"** column, with unique identification numbers matching those in the ***"category_id"*** column of the category DataFrame
   
   * The **"subcategory_id"** column, with the unique identification numbers matching those in the ***"subcategory_id"*** column of the subcategory DataFrame

2. Export the campaign DataFrame as campaign.csv and save it to your GitHub repository.

# Create the Contacts DataFrame

1. Use Python dictionary methods.

   * Import the `contacts.xlsx` file into a DataFrame.

   * Iterate through the DataFrame, converting each row to a dictionary.

   * Iterate through each dictionary, doing the following:

      * Extract the dictionary values from the keys by using a Python list comprehension.

      * Add the values for each row to a new list.

      * Create a new DataFrame that contains the extracted data.

      * Split each "name" column value into a first and last name, and place each in a new column.
      
      * Clean and export the DataFrame as `contacts.csv` and save it to your GitHub repository.

# Create the Crowdfunding Database

1. Inspect the four CSV files, and then sketch an ERD of the tables by using QuickDBDLinks to an external site.

![QuickDBD-Crowdfunding ETL](https://github.com/claytonmknight/Crowdfunding_ETL/assets/153461955/1eb5fe61-326e-463e-bbcd-3ff4f9425267)

2. Use the information from the ERD to create a table schema for each CSV file.

3. Save the database schema as a Postgres file named `crowdfunding_db_schema.sql`.

4. Create a new Postgres database, named `crowdfunding_db`.

5. Using the database schema, create the tables in the correct order to handle the foreign keys.

6. Verify the table creation by running a SELECT statement for each table.

7. Import each CSV file into its corresponding SQL table.

8. Verify that each table has the correct data by running a **SELECT** statement for each.

<img width="466" alt="Screenshot Contacts" src="https://github.com/claytonmknight/Crowdfunding_ETL/assets/153461955/c76bb488-87af-4ea9-9a9c-526b185d6f1c">

<img width="260" alt="Screenshot Category" src="https://github.com/claytonmknight/Crowdfunding_ETL/assets/153461955/c8653ec5-bc93-4dab-aa3d-f90822cc412d">

<img width="245" alt="Screenshot Subcategoy" src="https://github.com/claytonmknight/Crowdfunding_ETL/assets/153461955/65d67b80-88f9-488e-990e-4d2fd8ff343f">

<img width="758" alt="Screenshot Campaign" src="https://github.com/claytonmknight/Crowdfunding_ETL/assets/153461955/786551dd-f232-4c4a-82cd-ee2c66bd1d0e">
