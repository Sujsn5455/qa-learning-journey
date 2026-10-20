\# Day 20 — SQL JOINs



\## What is a JOIN?

Combines rows from two or more tables based on a related column.



\## Why QA Needs JOINs

Data is split across tables. The UI shows mixed data. To verify it in the database, you must JOIN tables.



\## Types of JOINs



\### INNER JOIN

Returns only rows with a match in BOTH tables.



```sql

SELECT customers.name, bookings.service\_name, bookings.price

FROM customers

INNER JOIN bookings ON customers.id = bookings.customer\_id;



LEFT JOIN

Returns ALL rows from the left table, and matches from the right. If no match, right columns are NULL.



sql

SELECT customers.name, bookings.service\_name

FROM customers

LEFT JOIN bookings ON customers.id = bookings.customer\_id;

RIGHT JOIN

Returns ALL rows from the right table, and matches from the left.



sql

SELECT customers.name, bookings.service\_name

FROM customers

RIGHT JOIN bookings ON customers.id = bookings.customer\_id;

JOIN with WHERE

sql

SELECT customers.name, bookings.service\_name

FROM customers

INNER JOIN bookings ON customers.id = bookings.customer\_id

WHERE customers.name = 'Sujan Karki';

JOIN with ORDER BY

sql

SELECT customers.name, bookings.service\_name, bookings.price

FROM customers

INNER JOIN bookings ON customers.id = bookings.customer\_id

ORDER BY bookings.price DESC;

