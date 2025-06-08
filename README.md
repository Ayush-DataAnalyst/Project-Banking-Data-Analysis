# 🏦 Banking Data Analysis Project

This project provides a comprehensive analysis of banking data using Python, SQL, and Power BI.
It covers all critical aspects of exploratory data analysis, SQL querying, and 
insightful visualizations to understand customer behavior, product performance, 
and overall banking operations.

## 🔧 Tools & Technologies Used

- **Python** 🐍 – For data cleaning, transformation, and exploratory data analysis (EDA)
- **SQL** 💾 – To query and analyze structured data
- **Power BI** 📊 – For creating dynamic dashboards and visualizations
- **Jupyter Notebook** 📓 – For interactive EDA and analysis
- **SQL-Python Integration** – Used libraries like `pyodbc`/`sqlalchemy`
  to connect and query SQL databases from Python

---

## 📁 Project Structure

Banking-Data-Analysis/
├── data/ # Contains raw & cleaned datasets
├── notebooks/ # Jupyter notebooks for EDA and SQL integration
├── sql/ # SQL query scripts
├── powerbi/ # Power BI dashboard files (.pbix)
├── reports/ # Exported analysis reports (optional)
└── README.md # Project documentation


---

## 🔍 Key Analyses Performed

- Customer segmentation and demographics
- Loan and credit product performance
- Deposit trends and customer balances
- Branch performance comparison
- Fraud detection trends (if applicable)
- Time-series analysis of transactions and customer activity

---

## 🔗 SQL-Python Integration

We used `pandas` along with `pyodbc` to run complex SQL queries directly within Python, 
enabling a hybrid approach of SQL filtering and Python-based visualization and modeling.

```python
import pandas as pd
import pyodbc

conn = pyodbc.connect('DRIVER={SQL Server};SERVER=your_server;DATABASE=your_db;UID=user;PWD=password')
query = "SELECT * FROM customer_data"
df = pd.read_sql(query, conn)
