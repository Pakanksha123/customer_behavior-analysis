# customer_behavior-analysis
Customer shopping behavior analysis using Python and MySQL, including data cleaning, preprocessing, database connection, SQL extraction, and customer purchase pattern analysis.
Overview

This project analyzes customer shopping behavior using Python and MySQL. The goal is to preprocess raw data, store it in a MySQL database, and extract useful insights such as customer purchase patterns, total spending, and product preferences. This project demonstrates practical skills in data preprocessing, database connectivity, SQL querying, and data analysis.

Technologies Used

Python

MySQL Server

MySQL Workbench

Pandas

NumPy

SQLAlchemy / PyMySQL

Jupyter Notebook

Features

Data preprocessing and cleaning

Handling missing and duplicate values

Connecting Python to MySQL database

Loading cleaned data into MySQL

Extracting data using SQL queries

Analyzing customer purchase behavior

Project Workflow

Load customer shopping dataset using Pandas

Perform data cleaning and preprocessing

Connect Python to MySQL server

Create database and tables in MySQL

Load cleaned data into MySQL database

Extract data using SQL queries

Analyze customer shopping behavior

Example Code
Connect Python to MySQL
from sqlalchemy import create_engine

engine = create_engine("mysql+pymysql://root:password@localhost:3306/customer_db")
Load Data into MySQL
df.to_sql("customer_shopping", con=engine, if_exists="replace", index=False)
Extract Data from MySQL
import pandas as pd

query = "SELECT * FROM customer_shopping"
data = pd.read_sql(query, engine)
Project Structure
Customer-Shopping-Behavior-Analysis/
│
├── data/
│   └── shopping_data.csv
│
├── notebooks/
│   └── analysis.ipynb
│
├── scripts/
│   └── database_connection.py
│
├── README.md
└── requirements.txt
Key Insights

Identified customer purchase patterns

Calculated total spending per customer

Analyzed product preferences

Extracted useful business insights from SQL database

Learning Outcomes

Data preprocessing using Python

Database connectivity using SQLAlchemy

Data storage and retrieval using MySQL

SQL query execution using Python

Customer behavior analysis using real-world data

Author

Akanksha
Python | SQL | Data Analysis | MySQL
