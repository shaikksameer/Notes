<<<<<<< HEAD
# ![picture](https://upload.wikimedia.org/wikipedia/commons/thumb/f/f3/Apache_Spark_logo.svg/2560px-Apache_Spark_logo.svg.png)

    * It is cluster computing platform designed to be fast and general purpose.
    * In memory computation (if i have 4 gb ram and my data is 8 gb then it will take 4 gb to ram to process and other 4 gb on  )
    * Designed to cover wide range of workload 

Cluster manager: 
    * hadoop yarn
    * apache Mesos
    * Standalone 

Spark supports many file format: 
    * Avro
    * Parquet 
    * csv etc 

Spark : 
    * RDD (are immutable)
    * Transformation (process of making rdd out of a rdd) 
    * Actions (c.collect)
    
>Spark architucture : 
    ![picture](https://avinash333.files.wordpress.com/2019/08/spark-architecture.png)

 
 ## Spark Core
    
    * Contains basic functionality of spark (task sheduling, memory management , fault recovery, interacting with storage system )
    * Home to API that defines RDDs

## Spark sql 

    * To process the structred data 
    * Supports many sources of data like Hive tables, parquet, json 

## Spark Streaming
    * to process the data in motion 


## RDD 

    * Lazy evaluation 
    * caching
    
## Transformation are 2 types

    - Narrow  (map, filter, sample, union....)
    - Wide  (intersection, join......)

## Partitioning 

    * By Default partition will be equal to number of block in hdfs 

## DAG 
    * Directed Acyclic Graph
    * Before calling any action spark keeps on making DAG 
    * After any action is called then the dag is submitted to the dag scheduler 
    * then it is spilted into stages
    * then all the set of stages in given to the task scheduler 
    * task schedular will get in contact with cluster manager 

## Spark Context 
    *  Same as ticket to a park,  spark context is a ticket to spark 
    * It can be used to create RDDs,accumulators and broadcast variable 

## Spark Architecture 

![picture](https://www.interviewbit.com/blog/wp-content/uploads/2022/06/Spark-Architecture-1024x551.png)


## spark context :
The Spark driver program is the one that creates SparkContext object in the application. As soon as we submit the spark job, the driver program runs the main() method of your application and creates DAG's representing the data flow internally.


