\# Day 22 — Database Validation Practice Queries



\## Setup

```sql

CREATE TABLE customers (id INTEGER PRIMARY KEY, name TEXT, email TEXT, city TEXT);

CREATE TABLE bookings (id INTEGER PRIMARY KEY, customer\_id INTEGER, service\_name TEXT, price INTEGER, status TEXT);



INSERT INTO customers (id, name, email, city) VALUES

(1, 'Sujan Karki', 'sujan@test.com', 'Kathmandu'),

(2, 'Ram Sharma', 'ram@test.com', 'Pokhara');



INSERT INTO bookings (id, customer\_id, service\_name, price, status) VALUES

(101, 1, 'Haircut', 800, 'Confirmed'),

(102, 1, 'Facial', 1500, 'Pending');

Validation Scenarios
Scenario 1: Count bookings
Expected: 2

sql
SELECT COUNT(*) FROM bookings WHERE customer_id = 1;
Scenario 2: Find cancelled bookings
Expected: Empty result

sql
SELECT * FROM bookings WHERE status = 'Cancelled';
Scenario 3: Verify price of Haircut
Expected: 800

sql
SELECT service_name, price FROM bookings WHERE service_name = 'Haircut';
Scenario 4: Approve a booking
Action: Update status of booking 102 to 'Confirmed'.

sql
UPDATE bookings SET status = 'Confirmed' WHERE id = 102;
Verify the update:

sql
SELECT * FROM bookings WHERE id = 102;
