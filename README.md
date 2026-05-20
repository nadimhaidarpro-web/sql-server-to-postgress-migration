# Preface

This project is about migrating entreprise data from SQL server into Postgres.

We will be using test 4 : 

- SQL
- Python
- Jupyternotebook


# Pseudo code 

## High level

1. Audit the data in SQL Server 
2. Extract data from SQL Server (SSMS)
3. Transform the data
4. Load the data in PostgreSQL
5. Validate the data after Migration
6. Generation a validation report

## Low level

- Create a .env file
- Load env variables
- Connect to SQL Server (pyodbc)
- Connect to Postgres (psycopg2)
- Audit the data
- For each table
- Get row count
- Extract all rows
- Transform the column names to lowercase
- Convert the data types
- Create tables in Postgres
- Load tables in Postgres
- Run post-data migration checks
- Generate validation report
