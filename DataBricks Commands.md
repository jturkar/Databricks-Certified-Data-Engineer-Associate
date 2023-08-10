### Q1. How to delete a folder in databricks "DBFS:/"?
Ans. %fs rm -r dbfs:/user/hive/warehouse/{folder_name}

###  Q2. How to determine if a table is a managed table vs external table? 
Ans. Run SQL command **DESCRIBE EXTENDED table_name** and check type

### Q3. How to Drop the customers database and associated tables and data?
Ans. DROP DATABASE customers **CASCADE**

### Q4. Define an external SQL table by connecting to a local instance of an SQLite database using JDBC

1. CREATE TABLE user_jdbc
2. USING org.apache.spark.sql.jdbc
3. OPTIONS (
4.        url = "jdbc:sqlite:/sqmple_db",
5.           dbtable = "users"
6.       )
     
