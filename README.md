# Data Modeling with Postgres

There is a startup called Sparkify who wants to analyze the data that they have been collecting. So, the aim of the project is to perform ETL of the data(JSON to a Postgres Database) that Sparkify has collected for easy analysis.The dataset used here is an subset of [Million songs Dataset](http://millionsongdataset.com/).<br>



## Database Design

Fact Table - `'songplays'` - records in log data associated with song plays. <br>
Columns - songplay_id, start_time, user_id, level, song_id, artist_id, session_id, location,<br> user_agent
<br><br>
Dimension Tables -
<br>
`users` - user_id, first_name, last_name, gender, level
<br>
`songs` - song_id, title, artist_id, year, duration
<br>
`artists` - artist_id, name, location, latitude, longitude
<br>
`time`- timestamps of records in songplays - start_time, hour, day, week, month, year, weekday
<br><br>

![alt txt](Db%20Design.jpg)

## Implementation Steps

<ol>
<li>Write SQL 'CREATE', 'DROP' and 'INSERT' statements in `sql_queries.py` and run <br>`create_tables.py` to run it.</li>
<li>Use `etl.ipynb` as a step by step guide to insert data one table at a time.</li>
<li>Use `test.ipynb` to check if the data is inserted or not.</li>
<li>Once all the steps are done, implement it in `etl.py` and run it to insert the whole data.</li>
</ol>

