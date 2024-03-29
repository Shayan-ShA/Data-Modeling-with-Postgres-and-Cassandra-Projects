<h2>Overview</h2> 

A startup called <b>Sparkify</b> wants to analyze the data they have been collecting on songs and user activity on their new music streaming app. The analytics team is particularly interested in understanding what songs users are listening to.

The aim is to create a Postgres Database Schema and ETL pipeline to optimize queries for song play analysis.

<h2>Project Description </h2>

In this project, I modeled data with Postgres and built an ETL pipeline using Python. On the database side, I defined fact and dimension tables for a Star Schema for a specific focus. On the other hand, ETL pipeline would transfer data from files located in two local directories into these tables in Postgres using Python and SQL.

<h2>Schema for Song Play Analysis</h2>

<b>Fact Table</b>

<b> songplays </b> records in log data associated with song plays

<b>Dimension Tables</b>

<b> users </b> in the app

<b> songs </b> in music database

<b> artists </b> in music database

<b> time: </b> timestamps of records in songplays broken down into specific units

<h2>Project Design</h2>

Database Design is very optimized because with a new number of tables and doing specific join, we can get the most information and do analysis

ETL Design is also simplified have to read json files and parse accordingly to store the tables into specific columns and proper formatting

<h2>Database Script</h2>

Writing "python create_tables.py" command in terminal, it is easier to create and recreate tables

<b>Jupyter Notebook</b>

etl.ipynb, a Jupyter notebook is given for verifying each command and data as well and then using those statements and copying into etl.py and running it into terminal using "python etl.py" and then running test.ipynb to see whether data has been loaded in all the tables

<h2>Relevant Files Provided </h2>

<b>test.ipynb </b>displays the first few rows of each table to let you check the database

<b>create_tables.py </b>drops and created your table

<b>etl.py </b>read and processes a single file from song_data and log_data and loads into your tables in ET

<b>sql_queries.py </b>containg all your sql queries and in imported into the last three files above

<h2>Environment</h2>
<ol>
 <li>Python 3.8</li>
 <li>PostgresSQL 12.8</li>
 <li>psycopg2 - PostgreSQL database adapter for Python</li>
</ol>

<h2>How to run</h2>
<p> Use SQL shell(psql) to create studentdb and sparkifydb postgres databases on your local machine</p>
<p>Run the following in Anaconda Promp(APP) in order</p>
 <ol>
  <li>python create_tables.py</li>
  <li>python etl.py</li>
 </ol>
<p>To make quieres and to check the databas, run test.ipynb in Jupyter Notebook</p>
