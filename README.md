# Crowdfunding_ETL
In this project, we extracted and transformed two csv files related to a fictional crowdfunding campaign website. Then, we took our transformed datasets, and loaded them into [PostgreSQL](https://www.postgresql.org/). We defined the database schema using [QuickDBD](https://www.quickdatabasediagrams.com/)

## Extract
---
In this step, we read the existing csv files contained in the "Resources" folder using [pandas](https://pypi.org/project/pandas/). After converting the existing data in both files to a pandas DataFrame, we then transformed the data into an acceptable state for importing into PostgreSQL.

## Transform
---
From the two starter files we were able to create four different csv files for loading. In the creation of those files, we:
- Made a category and subcategory table to help normalize the data
- Updated data types to integer, float, object, and datetime format
- Renamed columns for clarification and consistency
- Removed unnecessary columns from the DataFrames
- Exported the new, cleaned DataFrames to csv files for importing into PostgreSQL

## Load
---
After having all csv files ready for importation, we used QuickDBD to create the following table schema: ![Schema of Crowdfunding Database](https://github.com/QJones76/Crowdfunding_ETL/blob/main/data_output/crowdfunding_db_ERD.png)
We exported the code, created a database, created the four different tables, and loaded the csv files into the database. Then we checked to make sure our tables populated correctly. The output of the four tables is in the 'PostgreSQL table screenshots' folder. 
