# Introduction

## Introduction to the topic

### Data based on who creates them

- **Human-generated** (e.g., Social media ontent, emails, messages, documents)
- **Machine-generated** (e.g., DBMS log, sensor readings, network traces)

### Data based on their format

- **Structured** (e.g. Banking transactions, electronic health records)
  - Conforms to a data model or schema
  - Relational dataset/table
  - Can be manged using a DBMS

- **Unstructured** (e.g. Tweets, video files)
  - Does not conform to a model or schema
  - Textual or binary data
  - Stored as binary large objects (BLOBs) in a DBMS or in NoSQL databses

- **Semi-structured** (e.g. spreadsheets, XML data, sensor data, JSON data)
  - Non-relational data with a defined level of strcture or consistency
  - Hierarchical or graph-based

- **Metadata** (e.g. XML tags for the author and creation data of a document)
  - Provides information about a dataset's characteristics and structure
  - Data provenance

### Big Data Characteristics

1. **Volume**
  - Data quantity is substantial and evergrowing
  - Different storage and processing requirements
2. **Velocity**
  - Data speed may be high
  - Elastic and available time for processing
3. **Variety**
  - Multiple formats and types
  - Different integration, transformation, processing and storage requirements
4. **Veracity**
  - Bias, noise, abnormalities
  - Different requirements for removing noise and resolving invalid data
5. **Value**
  - Data usefulness(utility)
  - Depends on veracity, time of processing, storage & analysis decisions


## Data analytics & Big data

### Analytics

To infer knowledge that makes systems smarter & more efficient.

It involves: 

- Data filtering
- Processing
- Categorization
- Condensation
- Contextualization

### Analytic types

#### 1. Descriptive

Aim to answer **what** has happened, based on past data that are presented in a **summarized** form.

e.g.,

1. Basic statistics: Mean, Median, Variance, Count, Top-N, Distinct
2. Linear algebraic computations: Linear Regression, Principla Component Analysis, Singular Value Decomposition

#### 2. Diagnostic

Aim to answer **why** it has happened, based on past data

e.g.,

1. Clustering
2. Search shortest paths, minimum spanning tree

#### 3. Predictive

Aim to answer **what is likely to happen** based on existing data.

#### 4. Prescriptive

Aim to answer **what can we do to make something happen**, based on existing data

e.g.,

1. Optimization
2. Alignment problems

### Settings in Analytics

**Default**: the dataset is stored in RAM

**Streaming**: data arrive as a stream, a part (window) is stored

**Distributed**: data are distributed over multiple machines (in RAM and/or disk)

**Multi-threaded**: data are in one machine and multiple processors share the RAM of the machine




