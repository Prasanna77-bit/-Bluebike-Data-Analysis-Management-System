# 🚴‍♂️ Bluebike Data Analysis Management System (SQL-Only)

This project focuses on end-to-end data analysis of Boston’s Bluebike bike-sharing system using SQL. The objective is to derive actionable insights from raw trip data through structured querying, data cleaning, and aggregations.

---

## 📌 Project Overview

The Bluebike Data Analysis Management System is a SQL-powered analytical workflow designed to uncover trends in public bike usage. It leverages raw trip datasets and uses SQL queries to clean data, generate KPIs, and summarize behavioral and operational patterns.

---

## 🧠 Core Objectives

- Clean and normalize raw CSV trip data
- Write efficient SQL queries to extract key usage metrics
- Perform time-series and categorical analysis (e.g. by month, user type, gender)
- Identify high-traffic stations, peak hours, and trip duration patterns
- Support future dashboard or analytics integrations

---

## 🧰 Tools & Technologies

- **SQL**: Core language for data processing and analysis
- **Database Engine**: SQLite / PostgreSQL / MySQL (choose depending on setup)
- **Data Source**: Bluebike Trip History Data (CSV format)

---

## 📁 Project Structure

Bluebike-Data-Analysis-Management-System/
├── data/ # Raw Bluebike CSV files
├── sql/ # SQL scripts for cleaning and analysis
│ ├── 01_create_tables.sql
│ ├── 02_insert_data.sql
│ ├── 03_cleaning_queries.sql
│ ├── 04_analysis_queries.sql
├── outputs/ # Query outputs (CSV or TXT)
├── README.md # Project documentation

yaml
Copy
Edit

---

## ⚙️ How to Use

### 1. Load Data into SQL Database
- Create a new SQL database instance (SQLite, PostgreSQL, etc.)
- Run `01_create_tables.sql` to define schema
- Run `02_insert_data.sql` to load the CSV data into your tables

### 2. Clean and Preprocess
- Execute `03_cleaning_queries.sql` to:
  - Handle NULL values
  - Normalize station names
  - Filter invalid records (e.g. trips with negative duration)

### 3. Run Analytical Queries
- Use `04_analysis_queries.sql` to:
  - Calculate average trip durations
  - Identify peak usage hours
  - Segment data by user type (subscriber vs. casual)
  - Generate station-level traffic metrics

---

## 📊 Sample Analytical Questions Answered

- What are the busiest start stations?
- What are the average trip durations by customer type?
- What time of day sees the highest usage?
- Which months are most popular for biking?

---

## 📚 Data Source

Trip data retrieved from: [https://www.bluebikes.com/system-data](https://www.bluebikes.com/system-data)

---

## 🙋‍♂️ Author

**Prasanna Ganpat Pingale**  
Business Analyst | SQL Enthusiast  
📫 pingale.pr@northeastern.edu  
🔗 [LinkedIn](https://www.linkedin.com/in/prasannapingale)

---

## 📄 License

This project is licensed under the MIT License.

---

## 🛠 Future Enhancements

- Integration with BI tools like Power BI or Tableau
- Deployment of dashboard for non-technical stakeholders
- Automation of query outputs using scheduled scripts
