# ![picture](https://bigdatapath.files.wordpress.com/2019/03/3.png)
    MapReduce performs the processing of large data set in a distributed and parallel manner
  
* The MapReduce is a paradigm which has two phases, the mapper phase, and the reducer phase. In the Mapper, the input is given in the form of a key-value pair. The output of the Mapper is fed to the reducer as input.
* The reducer runs only after the Mapper is over. The reducer too takes input in key-value format, and the output of reducer is the final output.

* Two classes of MapReduce
    * Mapper 
    * Reducer

* Deamons : processes that run continuously in the background and perform functions required by other processes.

* Deaomons of MapReduce: 
    * Job tracker (boss)(Rescourse provider) (master) (schedule)
    * Task tracker (slave)


## process of mapreduce

> Input ->  splitting -> mapping -> shuffling -> reducing -> Final result 

 ![picture alt]( https://k21academy.com/wp-content/uploads/2021/10/Presentation1.jpg )


