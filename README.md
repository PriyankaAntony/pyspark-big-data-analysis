# pyspark-big-data-analysis
This work was completed as part of my M.Sc. in Computer Science at Clausthal University of Technology.
the work focuses on learning how large datasets can be processed using Apache Spark and PySpark.
The goal of the assignment was to understand distributed data processing and practice working with RDDs and DataFrames.

---

## Project Overview

In this project I worked on:

- Creating distributed datasets with PySpark  
- Filtering and transforming data  
- Performing a word count analysis  
- Removing common stop words from text  
- Working with Spark DataFrames  
- Analyzing a small stock dataset

---

# Task 1 – Working with RDD

In this task I explored **RDDs (Resilient Distributed Datasets)** in PySpark.
I created a list of numbers from **0 to 20,000** and converted it into an RDD using `parallelize()`.
The data was split into multiple partitions so Spark could process it in parallel.
Then I filtered the dataset to keep only **odd numbers** using a lambda function and displayed the first few results with `take(5)`.
This example helped me understand how Spark distributes computations compared to normal Python processing.

---

# Word Count with PySpark
I implemented a basic **word count analysis**.
Steps involved:
1. Load the text file  
2. Split lines into words  
3. Map each word to a count  
4. Aggregate the counts  
5. Sort the results  
Finally, I displayed the **25 most frequent words**.

---

# Removing Stop Words

Common words such as *the*, *and*, *to*, and *is* appear frequently but do not add much meaning.
To improve the results, these words were removed before sorting the remaining words.

---

# Task 2 – Working with DataFrames

The second part of the assignment focused on Spark DataFrames.
### RDD vs DataFrame vs Dataset

**RDD** – Low-level distributed data structure.  
**DataFrame** – Structured data with columns and optimized performance.  
**Dataset** – Extension of DataFrames with type safety.

---

## Stock Data Analysis

A CSV dataset containing stock information was loaded into Spark as a DataFrame.
The dataset was explored by:
- Checking column names  
- Viewing the schema  
- Generating summary statistics

---

### Creating a New Column

A new column called **HV Ratio** was created using:High Price / Volume
This demonstrates simple feature creation using Spark.

---

### Additional Analysis

Finally, the **maximum and minimum values of the trading volume** were calculated.

---

# What I Learned
Through this assignment I gained experience with:
- PySpark
- Distributed data processing
- Text analysis
- DataFrames in Spark
- Basic data exploration

---

