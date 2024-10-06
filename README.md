# Python and SQL Exercises Collection

## Table of Contents
1. [Introduction](#introduction)
2. [Getting Started](#getting-started)
3. [Exercise Overview](#exercise-overview)
4. [Technologies Used](#technologies-used)
5. [Usage](#usage)
6. [Contributing](#contributing)
7. [License](#license)

## Introduction
Welcome to the **Python and SQL Exercises Collection**! This repository features a comprehensive set of exercises designed to strengthen your skills in both Python programming and SQL database management. Through practical examples, users will gain experience in connecting to MySQL databases, executing SQL queries, and processing the results using Pandas.

## Getting Started
To get started with the exercises, follow these steps:

1. **Clone the repository**:
   ```bash
   git clone https://github.com/yourusername/python-sql-exercises.git
   cd python-sql-exercises
2. Install Required Packages: Make sure you have the necessary packages installed. You can install them using pip:
 pip install mysql-connector-python pandas

3. Set Up Database Connection: Update the connection parameters (host, database, user, password) in the notebook to connect to your MySQL database.

4. Open the Jupyter Notebook: Launch Jupyter Notebook and open Python_SQL_Exercises.ipynb.

5. Run the Notebook: Execute the cells in the notebook to work through the exercises and see the results.

## Exercise Overview
The exercises are structured to cover key aspects of using Python with SQL, including:

- Database Connection: Establishing a connection to a MySQL database.
- Executing Queries: Running various SQL queries to extract data.
- Data Extraction: Fetching and displaying results from SQL queries.
- Data Analysis: Utilizing Pandas for data manipulation and analysis.
- Advanced Queries: Implementing complex SQL queries for various use cases.

## Key Exercises Include:
- Connecting to a MySQL Database
- Fetching product listings from the database
- Querying orders based on specific criteria
- Analyzing employee salaries and order statistics
- Joining tables and aggregating data
- Exporting results to CSV files

## Technologies Used
- Python: The primary programming language used in the exercises.
- MySQL: The database management system for storing and querying data.
- Pandas: A data manipulation library used for processing query results.
- Jupyter Notebook: The environment for writing and executing the exercises.

## Usage
To execute the exercises, open the Jupyter Notebook file and run each cell sequentially. You can modify the SQL queries to explore different datasets and scenarios.

import mysql.connector
import pandas as pd

# Establishing the connection
connection = mysql.connector.connect(
    host='your_host',
    database='your_database',
    user='your_user',
    password='your_password',
    connection_timeout=180
)

# Executing a simple SQL query
query = "SELECT * FROM EMPLEADO;"
df_employees = pd.read_sql(query, con=connection)
print(df_employees.head())


### Author
- **Name**: Rosalía González Caviedes
- **Email**: rosaliagonzalezc@gmail.com
- [LinkedIn profile](https://www.linkedin.com/in/rosaliagonzalezcaviedes/)
- [Github profile](https://github.com/liagcaviedes)

### License
This project is licensed under the MIT License 

