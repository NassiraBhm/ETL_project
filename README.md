# ETL_project
📝 Project Summary: ETL Project with SQLAlchemy
In this project, I designed a simple ETL (Extract, Transform, Load) pipeline using Python, Pandas, and SQLAlchemy to manipulate and store product data from a public API.

📦 Data Source: FakeStoreAPI
The data was extracted from the free FakeStoreAPI, which simulates product information from an e-commerce website.

🔁 ETL Pipeline Steps
1. Extraction
The data was retrieved in JSON format via the API using the requests library.

2. Transformation
The JSON data was converted into a DataFrame using pandas. The nested rating field was separated into two separate columns: rating_rate and rating_count.

3. Loading
Using SQLAlchemy, I:

Created a local SQLite database (sales_data.db)

Defined a Product table model

Automatically created the table in the database

Inserted the cleaned data using a SQLAlchemy session

🔎 Data Querying
After loading, I ran SQL queries in Python using SQLAlchemy ORM to explore the data.
For example, I filtered products belonging to the "electronics" category using the .filter() method.

🎯 Objective
This project allowed me to:

Understand and implement a simple ETL process

Learn how to use SQLAlchemy for data modeling, insertion, and querying

Familiarize myself with manipulating data from an API
