# ETL_Challenge
Project Overview
 
This challenge required performing Extract-Transform-Load function on Kaggle and Wikipedia data for a streaming service Amazing Prime. The ETL steps performed were extracting data from Kaggle, transforming the data into a usable version then loading the dataset into PostgresSQL.
 
The objectives of this challenge are:
-       Create an automated ETL pipeline from raw data
-       Extract data from multiple sources
-       Clean and transform the data using Pandas
-       Use (Regex) regular expressions to parse the data
-       Load data into PostgreSQL database.
 
Extracting
Wikipedia Movies JSON file, started with 193 columns, Kaggle movie Metadata had 24 columns and Kaggle Ratings data had 26022489 rows and 4 columns. 
 
Transforming
Wikipedia movies was transformed to 22 columns after making the data concise and compact.
Wikipedia Movies was then merged with Kaggle Movies. This returned 6052 row counts. 
 
Loading 
The data was loaded to PostgresSQL to create a Movie Database in which a Movies Query and Ratings Query were executed.
 
The follow were the assumptions 

1.	The three (3) necessary data files are all stored in the same directory as declared in variable ‘fil-dir’. 
2.	The data will always have the accurate file format ie. .json or csv. The datatypes inside the files and file types must also be correct; as incorrect formats or files and file types could break the ETL pipeline.
3.	All spellings for columns names will remain the same throughout the datasets and will not be removed. There will be no new columns for future data.
4.	Numeric formatting such as dollars, dates, times will not change as this could affect the regular expression.
5.	The tables created in the SQL database will remain and the data will only be deleted and replaced instead of appending to the existing dataset.  
6.	Additional columns and categories for example TV Shows and Adult movies cannot be appended to the dataset without refactoring the function. 
7.	Future data will be consistent where the Kaggle data is more accurate. In that, the same antidote will be employed to correct data overlap between Wikipedia and Kaggle.


Summary
The JSON file along with two (2) Kaggle files were extracted, transformed and then joined. Subsequently, the movies and ratings files were then loaded into the database for the Amazing Prime services.
![image](https://user-images.githubusercontent.com/109915684/192070614-fb0cd5eb-4147-41ed-96ae-671136cfe0e6.png)
