# ![picture](https://upload.wikimedia.org/wikipedia/commons/thumb/b/b4/Apache_Sqoop_logo.svg/1280px-Apache_Sqoop_logo.svg.png)
    Sqoop is a tool designed to transfer data between Hadoop and relational database servers.

## Two main task 
    * Import 
        - Table row is sql == Record in hdfs file
    * Export 
        - Record in hdfs file == Row in sql table 


## Techinque 
    * To import the data sqoop initates MR job
    * By default there are 4 mappers 

##  Import Commands

    * Import table :
        $ sqoop import \    
        --connect jdbc:mysql://localhost/userdb \
        --username root \
        --table emp --m 1

    * Importing into Target Directory: 
        $ sqoop import \
        --connect jdbc:mysql://localhost/userdb \
        --username root \
        --table emp_add \
        --m 1 \
        --target-dir /queryresult

    * Import Subset of Table Data:
        $ sqoop import \
        --connect jdbc:mysql://localhost/userdb \
        --username root \
        --table emp_add \
        --m 1 \
        --where “city =’sec-bad’” \
        --target-dir /wherequery

    * Incremental Import:
        $ sqoop import \
        --connect jdbc:mysql://localhost/userdb \
        --username root \
        --table emp \
        --m 1 \
        --incremental append \
        --check-column id \
        -last value 1205 

    * Import all tables: 
         $ sqoop import-all-tables \
        --connect jdbc:mysql://localhost/userdb \
        --username root 

## Export command

    $ sqoop export \
    --connect jdbc:mysql://localhost/db \
    --username root \
    --table employee \ 
    --export-dir /emp/emp_data

