A startup called Sparkify wants to analyze the data they've been collecting on songs and user activity on their new music streaming app. We need to create a Postgres database and build an ETL pipeline for optimized querying and data handling.

For this project, we will create a star schema because it allows for quicker aggregations and fewer joins. Our fact table songlplays contain records in log data that are associated with song plays. The dimension tables are users, artists, songs, and time. 


How to Run:

1. Connect to the default postgres user student 
2. Run create_tables.py
3. Run etl.py
4. Look at results with test.ipynb


Project Structure:

/data - This is the folder that provides song and log files. 

create_tables.py - Drops the Sparkify database and its table and recreates them

etl.ipynb - Jupyter notebook of etl.py

etl.py - Parses all of the JSON objects in the song files and log files and then transforms the data to be later inserted into tables. 

sql_queries.py - Scripts that include creating tables, dropping tables, inserting rows into tables, and finding a song to be inserted into the songplay table

test.ipynb - Tests for correct insertions into the tables