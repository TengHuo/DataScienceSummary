# Data Processing: Spark

## Spark

- Unified engine for distributed data processing,
- Spark extends MapReduce programming model with an abstraction that allows efficient data reuse.

### Drawback of MapReduce

- Map Reduce is inefficient for applications that reuse intermediate results across multiple computations.
- Map Reduce is inefficient for interactive data mining (multiple ad-hoc queries on the same data)


## Overview of Resilient Distributed Datasets (RDDs)

- An RDD is a read-only, fault-tolerant collection of records that can be operated in parallel.
- An RDD is a data structure that serves as the core unit of data. User program can manipulate it, control its partitioning, make it persistent in memory.

### RDD vs. Distributed Shared Memory (DSM)

DSM: a global address space that applications can read and write to in arbitrary locations.

RDDs created by coarse-grained transformations (applied to the entire dataset) but reads can be fine-grained (read from a specific location).

DSM allows fine-grained writes and reads.

Thus, RDDs restricted to applications performing bulk writes.

### Advantages of RDD

1. RDDs provide efficient fault tolerance
  - They can be recovered using lineage
  - Only lost partitions need to be recomputed (and this can be done in parallel)
2. Spark can run backup copies of slow tasks (e.g., to address issues with slow nodes as in MapReduce) without accessing the same memory
3. Runtime can schedule tasks based on data locality to improve performance
4. RDDs degrade gracefully when there is not enough memory to store them. Partitions that do not fit in RAM stored on disk.

### Aplications for RDD

**Suitable** for batch applications that perform the same operation to the entire dataset.

- RDDs remember each transformation as one step in a lineage graph
- RDDs can recover lost partitions efficiently

**Not suitable** for applications that make asynchronous fine-grained updates to shared state.

- e.g., storage system for a web application in which many users update values on the same table

### Representing Dependencies



## pySpark

