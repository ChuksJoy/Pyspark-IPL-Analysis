# 🏏 IPL Data Analysis with PySpark on Databricks

This project demonstrates how to use **Apache Spark with PySpark on Databricks** to process, clean, analyze, and visualize cricket match data from the Indian Premier League (IPL). The dataset contains historical IPL match data up until 2017.

> 📊 [Click here to view the dataset on Data.World](https://data.world/raghu543/ipl-data-till-2017)

---

##  Project Objectives

The goal of this project is to showcase how PySpark can be used for:

- Reading and extracting data
- Structuring and cleaning raw data
- Performing exploratory analysis using Spark DataFrame operations
- Engineering new columns and formatting data
- Conducting aggregations and queries
- Visualizing the results directly in Databricks

---

##  Tools & Technologies

- **Apache Spark (PySpark)**
- **Databricks Notebook**
- **Python**
- **Spark SQL**
- **Matplotlib / Seaborn (for local visualization, if required)**
- **Data.World (Data Source)**

---

## Dataset Description

The dataset includes two CSV files:

1. **matches.csv** – Contains match-level data like team names, venue, match winner, toss details, etc.
2. **deliveries.csv** – Contains ball-by-ball delivery-level data for all IPL matches till 2017.

You can download the dataset from: [https://data.world/raghu543/ipl-data-till-2017](https://data.world/raghu543/ipl-data-till-2017)

---

## 📈 Key Features Implemented

### 1. 🔍 Reading and Loading Data
```python
df_matches = spark.read.csv("/path/to/matches.csv", header=True, inferSchema=True)
df_deliveries = spark.read.csv("/path/to/deliveries.csv", header=True, inferSchema=True)
