### Q1. How to delete a folder in databricks "DBFS:/"?
Ans. %fs rm -r dbfs:/user/hive/warehouse/{folder_name}

###  Q2. How to determine if a table is a managed table vs external table? 
Ans. Run SQL command **DESCRIBE EXTENDED table_name** and check type

### Q3. How to Drop the customers database and associated tables and data?
Ans. DROP DATABASE customers **CASCADE**

### Q4. Define an external SQL table by connecting to a local instance of an SQLite database using JDBC
CREATE TABLE user_jdbc
USING org.apache.spark.sql.jdbc
OPTIONS (
        url = "jdbc:sqlite:/sqmple_db",
          dbtable = "users"
       )
     
### Which of the following SQL statements can replace a python variable, when the notebook is set in SQL mode?
spark.sql(f"SELECT * FROM {schema_name}.{table_name}

### When writing streaming data, Spark’s structured stream supports the below write modes.
Append, Complete, Update

1. **Append mode(default)** - This is the default mode, where only the new rows added to the Result Table since the last trigger will be outputted to the sink.
2. **Complete Mode** -The whole Result Table will be outputted to the sink after every trigger. This is supported for aggregation queries. Target table is overwritten for each batch.
3. **Update Mode** -Only the rows in the Result Table that was updated since the last trigger will be outputted to the sink.

### A DELTA LIVE TABLE pipelines can be scheduled to run in two different modes, what are these two different modes?
Triggered, Continuous


