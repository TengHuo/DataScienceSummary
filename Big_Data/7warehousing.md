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

A new module in Apache Spark that integrates relational processing with Spark’s functional programming API. It lets Spark programmers leverage the benefits of relational processing (e.g., declarative queries and optimized storage). It lets SQL users call complex analytics libraries in Spark (e.g., machine learning).

### Motivation

1. Supporting **relational processing** both **within Spark programs** (on native RDDs) and **on external data sources** using a programmer-friendly API.
2. Providing **high performance using established DBMS** techniques.
3. Easily **supporting new data sources**, including semi-structured data and external databases amenable to query federation.
4. Enabling **extension with advanced analytics algorithms** such as graph processing and machine learning.











