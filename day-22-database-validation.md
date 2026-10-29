\# Day 22 — Database Validation for QA



\## What is Database Validation?

Checking the backend database to ensure UI actions correctly saved data, and that data matches the UI.



\## The QA Database Workflow

1\. \*\*UI Action:\*\* Perform an action in the website.

2\. \*\*UI Verification:\*\* Check the success message.

3\. \*\*DB Validation:\*\* Use SQL to verify the data in the database.

4\. \*\*Data Integrity:\*\* Check relationships between tables.



\## Common QA Bugs Found in DB

\- \*\*Missing Data:\*\* UI says success, but DB is empty.

\- \*\*Wrong Data:\*\* UI shows $50, DB shows $500.

\- \*\*Orphan Data:\*\* Customer deleted, but bookings remain.

\- \*\*Duplicate Data:\*\* User clicked once, DB shows two rows.



\## Essential Validation Queries



\### Count records

```sql

SELECT COUNT(\*) FROM bookings WHERE customer\_id = 1;



Verify status

sql

SELECT \* FROM bookings WHERE status = 'Cancelled';

Verify specific data (Price)

sql

SELECT service\_name, price FROM bookings WHERE service\_name = 'Haircut';

Update and Verify

sql

UPDATE bookings SET status = 'Confirmed' WHERE id = 102;

SELECT \* FROM bookings WHERE id = 102;

