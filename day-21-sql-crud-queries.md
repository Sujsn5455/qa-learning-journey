

\# Day 21 — SQL CRUD Practice Queries



\## Setup

```sql

CREATE TABLE customers (id INTEGER PRIMARY KEY, name TEXT, email TEXT, city TEXT);

CREATE TABLE bookings (id INTEGER PRIMARY KEY, customer\_id INTEGER, service\_name TEXT, price INTEGER, status TEXT);



INSERT INTO customers (id, name, email, city) VALUES

(1, 'Sujan Karki', 'sujan@test.com', 'Kathmandu'),

(2, 'Ram Sharma', 'ram@test.com', 'Pokhara'),

(3, 'Sita Thapa', 'sita@test.com', 'Kathmandu'),

(4, 'Hari Gurung', 'hari@test.com', 'Chitwan');



INSERT INTO bookings (id, customer\_id, service\_name, price, status) VALUES

(101, 1, 'Haircut', 800, 'Confirmed'),

(102, 1, 'Facial', 1500, 'Pending'),

(103, 2, 'Massage', 2000, 'Confirmed'),

(104, 3, 'Haircut', 800, 'Cancelled'),

(105, 4, 'Facial', 1500, 'Confirmed');

