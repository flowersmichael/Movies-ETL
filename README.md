# Movies-ETL
Predicting Hit Streaming Movies

## Overview
The fictitious company "Amazing Prime" would like to develop an algorithm to predict which low-budget releases will become popular, so that they can buy the streaming rights for a bargain.

## Process
For the company to develop the algorithm, we first needed to bring together data from multiple sources, and follow the ETL (Extract-Transform-Load) process to combine them into a clean dataset, and save them into a SQL database. 

### Extract
Here are the three sources we extract from:

* Wikipedia data stored as a JSON file. This contains data on movies made between 1990 and 2018, scraped from Wikipedia sidebars.
* A metadata file accessed on Kaggle that has details about movies from The Movie Database (TMDb) stored in CSVs 
* A MovieLens dataset, also accessed on Kaggle, of over 20 million ratings, stored in CSVs

### Transform
We used Python and Pandas to explore and transform the data.

### Load
We loaded our data into a PostgreSQL table.

## Results
We successfully cleaned up the Wikipedia and Kaggle data, and transformed them into tabular format with the right data types for each column. We then merged the data and cleaned the merged file, in particular the columns where the data overlapped. We then loaded it successfully into a SQL database.

Finally, we created an automated pipeline that takes in new data, performs the appropriate transformations, and loads the data into existing tables.

