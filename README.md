# DataModelingWithPostgres-Sparkify
 
### Table of Contents

1. [Project Overview](#summary)
2. [File Structure](#Files)
3. [Data Schema](#schema)
4. [Results of Optional Queriess](#results)
5. [Acknowledgements](#licensing)


    
## Project Overview<a name="summary"></a>

This project is part of Data Engineering Nano degree, which mainly focuses on a 

A startup called Sparkify wants to analyze the data they've been collecting on songs and user activity on their new music streaming app. The analytics team is particularly interested in understanding what songs users are listening to. Currently, they don't have an easy way to query their data, which resides in a directory of JSON logs on user activity on the app, as well as a directory with JSON metadata on the songs in their app.

They'd like a data engineer to create a Postgres database with tables designed to optimize queries on song play analysis, and bring you on the project. Your role is to create a database schema and ETL pipeline for this analysis. You'll be able to test your database and ETL pipeline by running queries given to you by the analytics team from Sparkify and compare your results with their expected results.

## File Structure<a name="Files"></a>

1. data folder: contains data files 
2. sql_queries.py: scripts to drop / create tables and insert data to tables
3. create_tables.py: creates the database and runs scripts in sql_queries.py to create tables
4. etl.ipynb: scripts to extract data from the data folder, transform and load data to the created tables
5. etl.py: runs scripts in etl.ipynb to extract, transforma and load data to our database
6. test.ipynb: scripts to select data from db and test performance as well as data exploration scripts

## Data Schema <a name="schema"></a>

following is a diagram that dipicts fact and dimension tables to represent a star schema:
![](sparkifySchema.png?raw=true)
            
    
## Results of Optional Queries<a name="results"></a>

1. We find that a free user played 5 songs only and a paid user played 61 songs, does that infer that Sparkify introduces a limit on song plays for free users?
2. SPARKIFY DB has 69 artists
3. SPARKIFY has 71 songs in DB
4. SPARKIFY has 96 users in DB although of a relatively low number of songs/artists
5. Most of SPARKIFY users are free users, where 78 are FREE and only 18 are PAID


## Acknowledgements<a name="licensing"></a>
Credits go to udacity for providing the opportunity to practice our skills!
