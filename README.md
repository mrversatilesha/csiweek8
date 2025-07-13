# 🚕 NYC Taxi Data Analysis with PySpark on Databricks

[![Demo Video](https://img.shields.io/badge/Watch-Demo-blue)](https://drive.google.com/file/d/1GKOc7kJo2pMNWRfuUgui7hAbNMXxrL9h/view?usp=sharing)

## 📌 Project Description

This project demonstrates how to load, process, and analyze NYC Yellow Taxi data using **PySpark** on **Azure Databricks**. It covers the full pipeline — from loading Parquet files, performing key data transformations, to running insightful analytical queries.

> 🗂 **Dataset Used:**  
> [yellow_tripdata_2018-01.parquet](https://d37ci6vzurychx.cloudfront.net/trip-data/yellow_tripdata_2018-01.parquet)

---

## 📊 Key Features and Queries Performed

### ✅ 1. Add a `Revenue` Column
Calculated revenue by summing:
fare_amount + extra + mta_tax + improvement_surcharge + tip_amount + tolls_amount + total_amount


### ✅ 2. Passenger Count by Area
Grouped trips by `PULocationID` to find areas with the highest passenger traffic.

### ✅ 3. Real-Time Vendor Earnings
Computed average fare and revenue amounts earned by each vendor.

### ✅ 4. Moving Count of Payments
Used window functions to get rolling counts of payments by each payment mode over recent entries.

### ✅ 5. Top 2 Earning Vendors by Date
Aggregated revenue, distance, and passenger count to find the top two vendors on any given date.

### ✅ 6. Busiest Route by Passenger Count
Found the most crowded route using `(PULocationID, DOLocationID)` grouped by `passenger_count`.

### ✅ 7. Top Pickup Locations (Last 10 Seconds)
Simulated a streaming query to identify top pickup locations using a 10-second window on timestamps.

---

## 🛠 Tech Stack

- 💻 **Platform:** Azure Databricks
- ⚡ **Language:** PySpark (Python)
- 📂 **Data Source:** NYC TLC Public Dataset (Parquet)
- 📦 **Libraries:** PySpark SQL, Window Functions, Pandas (for optional visualizations)

---

## 🎬 Demo Video

▶️ [Click here to watch the demo](https://drive.google.com/file/d/1GKOc7kJo2pMNWRfuUgui7hAbNMXxrL9h/view?usp=sharing)

---

## 🚀 How to Run the Project

1. Upload the Parquet file into Databricks (or connect directly via Azure Blob/ADLS).
2. Launch a Databricks cluster (11.3 LTS or higher recommended).
3. Import the notebook or paste code blocks from this repository.
4. Run each query cell-by-cell and visualize the insights.

---

