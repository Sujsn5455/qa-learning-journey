\# Day 24 — Decision Table \& State Transition Practice



\## Exercise 1: Salon Discount Rules

\*\*Rule:\*\*

\- If user is a VIP AND books Haircut -> 20% discount.

\- If user is a VIP AND books Facial -> 10% discount.

\- If user is NOT VIP AND books Haircut -> 5% discount.

\- If user is NOT VIP AND books Facial -> 0% discount.



\### Decision Table:

| Rules | R1 | R2 | R3 | R4 |

|-------|----|----|----|----|

| VIP? | Yes | Yes | No | No |

| Service = Haircut? | Yes | No | Yes | No |

| \*\*Discount\*\* | 20% | 10% (Facial) | 5% | 0% |



\## Exercise 2: State Transition for Booking

Draw the state diagram for a booking:

1\. User creates booking (State: Pending).

2\. Admin confirms (State: Confirmed).

3\. User cancels (State: Cancelled).

4\. Admin rejects (State: Rejected).



\### Test Scenarios:

1\. Pending -> Confirmed (Valid)

2\. Pending -> Cancelled (Valid)

3\. Pending -> Rejected (Valid)

4\. Confirmed -> Cancelled (Valid)

5\. Cancelled -> Confirmed (INVALID - should throw error)

6\. Rejected -> Confirmed (INVALID)



\## What I Learned

\- How to build a decision table for complex rules.

\- How to draw state transitions for workflows.

\- How to identify invalid transitions that cause bugs.



\## Key Takeaway

Testing combinations and workflows ensures no edge cases are missed.

