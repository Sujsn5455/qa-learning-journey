\# Day 2 — SDLC vs STLC + Testing Types



\## SDLC (Software Development Life Cycle)



\*\*Definition:\*\*

SDLC is the process of building software from start to finish.



\*\*Phases:\*\*

1\. Requirement Gathering - What client wants

2\. Analysis - Team studies feasibility

3\. Design - System architecture and UI

4\. Development - Developers write code

5\. Testing - Testers verify the product

6\. Deployment - Product goes live

7\. Maintenance - Fix bugs and updates



\*\*Salon Booking System Example:\*\*

\- Requirement: Salon owner wants online booking

\- Analysis: Team checks what is possible

\- Design: Design booking flow and database

\- Development: Developers build the app

\- Testing: Testers test login, booking, payment

\- Deployment: App goes live

\- Maintenance: Fix bugs reported by users



\---



\## STLC (Software Testing Life Cycle)



\*\*Definition:\*\*

STLC is the process of testing software. It is a subset of SDLC.



\*\*Phases:\*\*

1\. Requirement Analysis - Tester reads and reviews requirements

2\. Test Planning - Tester writes test plan and estimates effort

3\. Test Case Design - Tester writes test cases

4\. Test Environment Setup - Prepare environment and test data

5\. Test Execution - Run test cases, log bugs

6\. Test Closure - Write summary report



\*\*Salon Booking System Example:\*\*

\- Requirement Analysis: Tester reads booking requirements, finds gaps

\- Test Planning: Plan 50 test cases for booking flow

\- Test Case Design: Write test cases for login and booking

\- Environment Setup: Set up test database with dummy salons

\- Test Execution: Run tests, find bug in time slot selection

\- Test Closure: Report 10 bugs found, 8 fixed



\---



\## SDLC vs STLC Comparison



| SDLC | STLC |

|------|------|

| Covers entire development | Covers only testing |

| All teams involved | Mainly QA team |

| Starts with requirement gathering | Starts with requirement analysis |

| Ends with maintenance | Ends with test closure |

| Broader scope | Narrower scope |



\---



\## Testing Types



\### 1. Unit Testing

\- \*\*Definition:\*\* Testing individual functions or methods

\- \*\*Who:\*\* Developers

\- \*\*When:\*\* During development

\- \*\*Salon Example:\*\* Testing calculatePrice() method for booking cost



\### 2. Integration Testing

\- \*\*Definition:\*\* Testing how two or more modules work together

\- \*\*Who:\*\* Developers or testers

\- \*\*When:\*\* After unit testing

\- \*\*Salon Example:\*\* Testing booking + payment + email together



\### 3. System Testing

\- \*\*Definition:\*\* Testing the complete system end to end

\- \*\*Who:\*\* Testers

\- \*\*When:\*\* After integration testing

\- \*\*Salon Example:\*\* Login → select service → book → pay → confirmation



\### 4. UAT (User Acceptance Testing)

\- \*\*Definition:\*\* Client verifies the system meets business needs

\- \*\*Who:\*\* End users or client

\- \*\*When:\*\* Before going live

\- \*\*Salon Example:\*\* Salon owner tests admin panel to manage bookings



\### 5. Smoke Testing

\- \*\*Definition:\*\* Quick check that the build is stable

\- \*\*Who:\*\* Testers

\- \*\*When:\*\* After every new build

\- \*\*Salon Example:\*\* Login → book appointment → logout



\### 6. Regression Testing

\- \*\*Definition:\*\* Re-testing old features after new changes

\- \*\*Who:\*\* Testers

\- \*\*When:\*\* After code changes

\- \*\*Salon Example:\*\* After adding new payment option, verify login still works



\---



\## Test Pyramid

/UAT\\ ← Few

/------

/ System \\ ← Some

/----------

/ Integration\\ ← More

/--------------

/ Unit Testing \\ ← Many





Bottom to top: Unit → Integration → System → UAT



More unit tests. Fewer UAT.



\---



\## Key Takeaway



SDLC covers entire software development. STLC covers only testing. Testing has 6 main types, each with a specific purpose in the project lifecycle.



\---



\## Salon Project Questions



1\. Salon app SDLC phases: Requirement, Analysis, Design, Development, Testing, Deployment, Maintenance

2\. Salon app STLC phases: Requirement Analysis, Test Planning, Test Case Design, Environment Setup, Test Execution, Test Closure

3\. Unit test for login: Developer tests the login() method

4\. Integration test: Booking + Payment + Email together

5\. Smoke test: After new build, test login and booking quickly

6\. Regression test: After code change, verify old features still work

7\. UAT: Salon owner tests the app before going live



\---



\## One-Line Summary



SDLC builds the software. STLC tests the software.

