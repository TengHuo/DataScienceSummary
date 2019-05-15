# Networks and Graphs

## Overview



## Network Properties

### Degree distributions, P(k)

- Probability that a randomly chosen node has degree k
- $N(k)$ = number of nodes with degree k
- $P(k) = \frac{N(k)}{n}$

### Distance

**Distance** between a pair of nodes is defined as the number of edges along the shortest path connecting those nodes.

### Diameter and average path length

Let **h(i, j)** denote the length of the **shortest path** between node i and j (or the **distance** between i and j). The **diameter of a network** is the **largest** distance between any two nodes in the network:

$$
diameter = max\ h(i, j)
$$

The average path length is the average distance between any two nodes in the network.

$$
average\ path\ length = \frac{\sum_{i\leq j}h(i,j)}{0.5n(n-1)}
$$

Average path length is bounded from above by the diameter; in some cases, it can be much shorter than the diameter.

### Clustering Coefficient

What portion of i's neighbors are connected

Node i with degree $k_i$

$$
C_i = \frac{2e_i}{k_i(k_i - 1)}
$$

where $e_i$ is the number of edges between the neighbors of node i

Average clustering

$$
C = \frac{1}{N}\sum_i^NC_i
$$

## Sub-graphs and network algorithms

### Sub-graphs

### Spanning Tree

## Random Graphs & Erdos-Renyi model of random graph

### Random Graphs

### Isoloated Nodes

### Evolution of Random Graphs


























