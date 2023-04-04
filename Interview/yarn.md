# ![picture](https://www.datanami.com/wp-content/uploads/2017/05/hadoop-yarn.png)
    Yarn is the resourse management tool of the hadoop system. From hadoop 2.X  the Yarn has introduced . It shedules jobs and assigns resources 

> Yarn 2.0  supports

* Scalability  
* Compatibility
* Resource utilization 
* Multitenancy 

> Worloads running on Yarn 

* Mapreduce
* Tez
* Hbase
* Storm
* Graph 
* Spark 
* weave 
 - - - 

YARN architecture

1. Client submits an application
1. The Resource Manager allocates a container to start the Application Manager
1. The Application Manager registers itself with the Resource Manager
1. The Application Manager negotiates containers from the Resource Manager
1. The Application Manager notifies the Node Manager to launch containers
1. Application code is executed in the container
1. Client contacts Resource Manager/Application Manager to monitor application’s status
1. Once the processing is complete, the Application Manager un-registers with the Resource Manager

![picture](https://media.geeksforgeeks.org/wp-content/uploads/Application_WorkFlow_YARN.jpg)

 