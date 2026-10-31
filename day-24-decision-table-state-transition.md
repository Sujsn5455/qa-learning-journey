\# Day 24 — Decision Table \& State Transition Testing



\## 1. Decision Table Testing

Used when multiple conditions combine to create different outcomes.



\### Example: Salon Login

\- Condition 1: Correct Email?

\- Condition 2: Correct Password?



| Rules | R1 | R2 | R3 | R4 |

|-------|----|----|----|----|

| Correct Email? | Yes | Yes | No | No |

| Correct Password? | Yes | No | Yes | No |

| \*\*Action\*\* | Login Success | Error: Wrong Pass | Error: Wrong Email | Error: Wrong Email |



\## 2. State Transition Testing

Used when a system changes states based on events.



\### Salon Booking States:

\- \*\*Pending:\*\* Booking created, waiting for admin.

\- \*\*Confirmed:\*\* Admin approved.

\- \*\*Cancelled:\*\* Customer or Admin cancelled.



\### Valid Transitions:

\- Pending -> Approve -> Confirmed

\- Pending -> Cancel -> Cancelled

\- Confirmed -> Cancel -> Cancelled



\### Invalid Transitions (These are bugs!):

\- Cancelled -> Approve -> Confirmed (Cannot approve a cancelled booking)

\- Confirmed -> Approve -> Confirmed (Already approved)



\## QA Applications

\- Decision tables ensure 100% combination coverage.

\- State transition catches bugs in workflow logic.



\## Key Takeaway

Decision tables handle complex rules. State transition handles workflows. Both are essential for deep QA.

