# Hadoop MapReduce & Hive Data Warehousing System

A distributed batch processing implementation using Hadoop MapReduce and Apache Hive for large-scale data analytics, featuring HQL queries, data aggregation, and the classic WordCount algorithm on HDFS.

## 🎯 Project Overview

This project demonstrates practical implementation of the Hadoop ecosystem for processing and analyzing large datasets. Built a complete data warehousing solution using Apache Hive for SQL-like querying on top of Hadoop's distributed file system (HDFS), combined with custom MapReduce jobs for batch processing workflows.

## 🛠️ Technology Stack

- **Apache Hadoop** - Distributed storage and processing framework
- **Apache Hive** - Data warehouse infrastructure with HQL support
- **HDFS** - Hadoop Distributed File System for scalable storage
- **MapReduce** - Parallel processing paradigm for batch jobs
- **Java** - MapReduce job implementation
- **Apache Derby** - Embedded database for Hive metadata
- **HQL** - Hive Query Language for data operations

## 📋 Core Implementations

### Hive Data Warehousing

**Database & Schema Design:**
- Created structured databases using Hive DDL commands
- Designed tables with multiple fields for relational data storage
- Implemented proper data types and schema validation

**Data Manipulation:**
- Populated tables using `INSERT INTO` statements
- Performed CRUD operations on distributed datasets
- Managed data across HDFS through Hive abstraction layer

**Query Operations:**
- Basic retrieval with `SELECT` statements
- Conditional filtering using `WHERE` clauses
- Column projection for optimized data access
- Data aggregation with `COUNT()` functions
- Grouping and summarization with `GROUP BY`

### MapReduce Processing

**WordCount Implementation:**
- Developed classic MapReduce job in Java
- Implemented Mapper class for tokenization
- Built Reducer class for word frequency aggregation
- Configured job execution on Hadoop cluster

**Batch Processing Workflow:**
- Read input files from HDFS
- Distributed processing across cluster nodes
- Parallel computation for scalability
- Output results back to HDFS

### HDFS Operations

- Uploaded Nginx log files to distributed file system
- Managed file replication and fault tolerance
- Configured appropriate block sizes for optimization
- Verified data integrity across cluster

## 💡 Technical Highlights

### SQL-Like Analytics on Big Data
```sql
-- Data retrieval with filtering
SELECT * FROM authors WHERE id > 2;

-- Projection of specific columns
SELECT name, book_title FROM authors;

-- Aggregation and counting
SELECT COUNT(*) FROM authors;

-- Grouping with aggregation
SELECT name, COUNT(*) AS book_count 
FROM authors 
GROUP BY name;
```

### Distributed Architecture
- **Hive Metastore**: Metadata management with Derby
- **Query Execution**: HQL translation to MapReduce jobs
- **Storage Layer**: HDFS for distributed data persistence
- **Processing Layer**: MapReduce for parallel computation

### Key Capabilities
- Batch processing of large-scale datasets
- SQL interface for non-programmers (HQL)
- Schema-on-read flexibility
- Fault-tolerant distributed storage
- Horizontal scalability through partitioning

## 📊 Results & Validation

**Successful Operations:**
- Initialized Hive environment with proper configuration
- Created databases and tables in distributed warehouse
- Inserted and queried structured data successfully
- Executed MapReduce jobs on HDFS
- Performed aggregations and grouping operations
- Validated data consistency across cluster

**Data Processing Achievements:**
- Processed log files using MapReduce paradigm
- Demonstrated word frequency analysis at scale
- Executed complex HQL queries with joins and aggregations
- Managed metadata through Hive metastore

## 🚀 Skills Demonstrated

- **Distributed Systems**: Hadoop cluster configuration and management
- **Data Warehousing**: Hive architecture and HQL proficiency
- **Batch Processing**: MapReduce programming model
- **Java Development**: Custom MapReduce job implementation
- **Query Optimization**: Efficient data retrieval strategies
- **File System Management**: HDFS operations and administration
- **Problem Solving**: Debugging configuration and runtime errors

## 🏗️ System Architecture

**Data Flow:**
1. Raw data ingestion into HDFS
2. Hive table creation and schema definition
3. Data loading and validation
4. Query execution through Hive
5. MapReduce job translation and execution
6. Result aggregation and storage

**Components:**
- **Storage**: HDFS with configurable replication
- **Metadata**: Derby database for Hive metastore
- **Processing**: MapReduce framework
- **Interface**: Hive shell for HQL execution

## 📄 Technical Documentation

For complete implementation details, code samples, query examples, and system configurations, see the [full project documentation](PROJECT_PDF_NAME.pdf).

## 🎓 Background

Developed this project to gain hands-on experience with Hadoop ecosystem tools used in production data engineering workflows. Explored both MapReduce programming and SQL-like querying patterns essential for processing large-scale datasets in distributed environments similar to those used at companies like Yahoo, Facebook, and Netflix.

## 🔗 Connect

**Meriem Lmoubariki**
- GitHub: [@myriamlmiii](https://github.com/myriamlmiii)

---

*Demonstrating proficiency in distributed batch processing, data warehousing, and the Hadoop ecosystem.*
