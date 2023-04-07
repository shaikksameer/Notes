# ![picture](https://geekflare.com/wp-content/uploads/2022/11/Hive.png)

> Hive architecture
    ![picture](https://static.javatpoint.com/hadooppages/images/hive-architecture.jpg)

## Thrift Server :
    Thrift comes in the architectural part of Hive, Thrift is a protocol for the application which were developed in a different programming languages to communicate. So the Thrift server sits in a hive services layer and this is the one which receives the request or hive queries from client programs.

## HWI 
    Hive web interface 

## CLI 
    Command Line interface 

## Driver 
    It manages the lifecycle of the queries written in HWI, CLI or through thrift server
## MetaStore
    Store all the meta data of the table created 

## limitation of hive 
    * Not recommended for row level update 
    * Latency for hive query is high
    * Not designed for OLTP

> Diff with traditional rdbms
    
    schema on read vs schema on write


## Complex Data types
    * Strut
    * Maps
    * Array 

## Types of tables in HIVE 

    * Internal table
    * External Table 

   