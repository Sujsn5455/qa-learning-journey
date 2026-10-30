\# Day 23 — Test Design Techniques (EP \& BVA)



\## Why Test Design Techniques?

Writing test cases randomly is not enough. We need a scientific way to find the most bugs with the fewest test cases.



\## 1. Equivalence Partitioning (EP)

Divide input data into groups (partitions) that should behave the same way. Test one value from each group.



\### Example: Age field (Valid: 18 to 60)

\- Partition 1 (Invalid): Below 18

\- Partition 2 (Valid): 18 to 60

\- Partition 3 (Invalid): Above 60

\*Test Data:\* 10, 30, 70 (One from each)



\## 2. Boundary Value Analysis (BVA)

Bugs are usually found at the edges (boundaries) of valid ranges. Test the min, max, and just outside them.



\### Example: Age field (Valid: 18 to 60)

\- Min - 1 = 17 (Invalid)

\- Min = 18 (Valid)

\- Min + 1 = 19 (Valid)

\- Max - 1 = 59 (Valid)

\- Max = 60 (Valid)

\- Max + 1 = 61 (Invalid)



\## Salon Project Application

\*\*Rule:\*\* Appointment can be booked 1 to 30 days in advance.



\### EP for Salon Booking:

\- Invalid: Past dates

\- Valid: 1 to 30 days

\- Invalid: 31+ days



\### BVA for Salon Booking:

\- Min - 1 = Today (0 days) → Invalid

\- Min = Tomorrow (1 day) → Valid

\- Min + 1 = Day after tomorrow (2 days) → Valid

\- Max - 1 = 29 days → Valid

\- Max = 30 days → Valid

\- Max + 1 = 31 days → Invalid



\## Key Takeaway

EP reduces the number of test cases. BVA finds the hidden bugs at the edges. Use both together.

