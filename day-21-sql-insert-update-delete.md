\# Day 21 — SQL INSERT, UPDATE, DELETE



\## 1. INSERT (Add Data)

Adds new rows to a table.



```sql

INSERT INTO customers (id, name, email, city) 

VALUES (5, 'Gita Neupane', 'gita@test.com', 'Lalitpur');

2\. UPDATE (Modify Data)

Changes existing data.



⚠️ WARNING: Always use WHERE! If you forget WHERE, you will update every row.



sql

UPDATE customers 

SET city = 'Bhaktapur' 

WHERE id = 5;

3\. DELETE (Remove Data)

Removes rows from a table.



⚠️ WARNING: Always use WHERE! If you forget WHERE, you will delete all data.



sql

DELETE FROM customers 

WHERE id = 5;

