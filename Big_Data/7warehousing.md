# Big Data Warehousing

## Hive

An open-source data warehousing solution built on top of Hadoop, which supports queries that are

1. expressed in HiveQL (an SQL-like declarative language)
2. compiled into MapReduce jobs that are executed using Hadoop

### Applications

- Log processing
- Text mining
- Document indexing
- Customer-facing business intelligence (Google analytics)
- Predictive modeling
- Hypothesis testing

### Components of HIVE

1. Client components
2. Driver
3. Compiler
4. Optimizer
5. Executor
6. Metastore
7. Thrift Server


### Pros

- A easy way to process large scale data
- Support SQL-based queries
- Provide more user defined interfaces to extend
- Programmability
- Efficient execution plans for performance
- Interoperability with other database


### Cons

- No easy way to append data
- Files in HDFS are immutable



## SparkSQL

