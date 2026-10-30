\# Day 23 — Test Design Practice (EP \& BVA)



\## Scenario 1: Password Length

\*\*Rule:\*\* Password must be exactly 8 to 15 characters.



\### EP (Equivalence Partitioning)

\- Invalid: Less than 8 chars

\- Valid: 8 to 15 chars

\- Invalid: More than 15 chars



\### BVA (Boundary Value Analysis)

\- 7 chars (Invalid)

\- 8 chars (Valid)

\- 9 chars (Valid)

\- 14 chars (Valid)

\- 15 chars (Valid)

\- 16 chars (Invalid)



\## Scenario 2: Salon Service Price

\*\*Rule:\*\* Service price can be Rs 500 to Rs 5000.



\### EP

\- Invalid: Below 500

\- Valid: 500 to 5000

\- Invalid: Above 5000



\### BVA

\- 499 (Invalid)

\- 500 (Valid)

\- 501 (Valid)

\- 4999 (Valid)

\- 5000 (Valid)

\- 5001 (Invalid)



\## Scenario 3: Booking Time Slot

\*\*Rule:\*\* Booking time must be between 09:00 AM and 06:00 PM.



\### EP

\- Invalid: Before 09:00 AM

\- Valid: 09:00 AM to 06:00 PM

\- Invalid: After 06:00 PM



\### BVA

\- 08:59 AM (Invalid)

\- 09:00 AM (Valid)

\- 09:01 AM (Valid)

\- 05:59 PM (Valid)

\- 06:00 PM (Valid)

\- 06:01 PM (Invalid)



\## What I Learned

\- How to divide data into valid and invalid groups.

\- How to pick test data from the edges.

\- How to apply EP and BVA to the Salon project.



\## Key Takeaway

Test Design Techniques help you find bugs faster without wasting time on random testing.

