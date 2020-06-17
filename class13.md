[Table of Contents](https://github.com/logantscott/june2020_reading)

## Mongo Aggregations
These are like SQL's aggregate functions (count/sum/min/max/avg/etc). In mongo, they run through the aggregation pipeline, with each stage of the pipeline transforming the data to eventually get the output that is being requested.  

The match stage is basically saying select * where _____,  
```{ $match: { status: "A" } },```  
The group stage is group by, and contains the aggregation method in mongo  
```{ $group: { _id: "$cust_id", total: { $sum: "$amount" } } }```  
