# MapReduce Program (wordcount) 

* Every thing in mapreduce is key value pair 

>Example : 

    Input file :
        I am the best there is at what I do 
        but what I do isnt very nice

    Mapper Input : 
        0, I am the best there is at what I do
        36, but what I do isnt very nice

    Mapper Output: 
        I,1
        am,1
        the,1
        best,1
        ....
    Reducer Input
        I, [1,1,1]
        am, [1]
        .....
    Reducer Output
        I,3 
        am,1
        the,1
        ......
    