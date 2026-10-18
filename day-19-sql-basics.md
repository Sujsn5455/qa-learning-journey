\# Day 19 — SQL Basics: SELECT, WHERE, ORDER BY



\## What is SQL?

SQL (Structured Query Language) is used to interact with relational databases.



\## Why QA Needs SQL

Checking the UI is not enough. You must verify that data is correctly saved in the database.



\## Core Commands



\### SELECT

Reads data from a table.

```sql

SELECT \* FROM customers;       -- All columns

SELECT name, email FROM customers; -- Specific columns

