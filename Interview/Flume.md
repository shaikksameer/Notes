# ![picture](https://upload.wikimedia.org/wikipedia/en/1/1d/Apache_Flume_Logo.svg)
    Flume is a tool/service/data ingestion mechanism for collecting aggregating and transporting large amounts of streaming data such as log files, events (etc...) from various sources to a centralized data store.

* Advantage of flume 
    * scalable 
    * reliable
    * Real-time data streaming
    * Large data set 

## Flume architecture :
![picture](https://www.cloudduggu.com/flume/architecture/flume_architecture.png)

* Flume can not do transformation


* Flume conf file is know as Agent 
    * Agent => source(facebook, twitter api,web server) + channel(required  ram)  +sink(hdfs)  

## Flume only one command 
`> flume-ng agent -c <source file path> -f <conf file path> -n flatfile_agent`

 File name in flume will be the timestamp 

For more than one source we need to create more than one conf file in flume 