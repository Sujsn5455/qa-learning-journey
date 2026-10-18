

\## Database Setup (Salon System)

```sql

CREATE TABLE customers (

&#x20;   id INTEGER PRIMARY KEY,

&#x20;   name TEXT,

&#x20;   email TEXT,

&#x20;   city TEXT

);



CREATE TABLE bookings (

&#x20;   id INTEGER PRIMARY KEY,

&#x20;   customer\_id INTEGER,

&#x20;   service\_name TEXT,

&#x20;   price INTEGER,

&#x20;   status TEXT

);



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

