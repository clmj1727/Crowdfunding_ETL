# Crowdfunding_ETL

  * Category and Subcategory Dataframes
      * Extract and transfrom the data from crowdfunding.xlsx excel data to have a "category_id" column and a "category" column
      * Export the category dataframe as category.csv and saved to the repository
      * Extract and transform the data from crowdfunding.xlsx excel data to have a "subcategory_id" column and a "subcategory" column
      * Export the subcategory dataframe as subcategory.csv and saved to the repository
  * Campaign Dataframe
      * Extract and transform the data from crowdfunding.xlsx excel data to have the following columns:
          * "cf_id" 
          * "contact_id"
          * "company_name"
          * "blurb" rename to "description"
          * "goal" - convert to the float data type
          * "pledged" - convert to the float data type
          * "outcome"
          * "backers_count"
          * "country"
          * "currency"
          * "launched_at" - rename to "launch_date" and convert from UTC times to the datetime format
          * "deadline" - rename to "end_date" and convert from UTC times to the datetime format
          * "category_id" - with unique id numbers matching the "category_id" column from the Category Dataframe
          * "subcategory_id" - with unique id numbers matching the "subcategory_id" column from the Subcategory Dataframe
      * Export the Campaign Dataframe as campaign.csv and save it to the repository
  * Contacts Dataframe
      * Option 1:
          * Import the contacts.xlsx file into a dataframe
          * Iterate through the dataframe, converting each row to a dictionary
          * Iterate through each dictionary to extract the dictionary values from the keys by using a Python list comprehension and add the values for each row to a new list
          * Create a new dataframe that contains the extracted data
          * Split each "name" column value into a first and last name and place each in a new column
          * Clean and export the Dataframe as contacts.csv and save it to the repository
  * Crowdfunding Database
      * Inspect the 4 CSV files and sketch an ERD of the tables
      * Use the information from the ERD to create a table schema for each CSV file
      * Save the database schema as a Postgres file named crowdfunding_db_schema.sql and save it to the repository
      * Create a new Postgres database named crowdfunding_db
      * Using the schema, create the tables in the correct order to handle the foreign keys
      * Verify the table creation by running a SELECT statement for each table
      * Import each CSV file into its corresponding SQL table
      * Verify that each table has the correct data by running a SELECT statement for each

