\# Test Plan — Salon Booking and Customer Management System



\## 1. Test Plan ID

TP-SALON-001



\## 2. Introduction

This document describes the test plan for the Salon Booking and Customer Management System. It covers the scope, approach, resources, and schedule of testing activities for login, registration, booking, payment, and admin modules.



\## 3. Scope



\### In Scope

\- User Login

\- User Registration

\- Service Selection

\- Appointment Booking

\- Payment

\- Booking Cancellation

\- Admin Panel (manage bookings, services)

\- Email Notifications



\### Out of Scope

\- Third-party payment gateway internals

\- Email server infrastructure

\- Native mobile apps (web only for now)

\- Performance testing under heavy load

\- Security penetration testing



\## 4. Objectives

\- Verify all functional requirements of the Salon system

\- Ensure login and registration work correctly

\- Validate booking flow end to end

\- Confirm payment processing works

\- Test admin panel functionality

\- Report all defects clearly

\- Achieve 95% test case pass rate before release



\## 5. Test Strategy



\### Types of Testing

\- Unit Testing — developers test individual functions

\- Integration Testing — booking + payment + email together

\- System Testing — full end-to-end flow

\- Smoke Testing — after every new build

\- Regression Testing — after code changes

\- UAT — Salon owner tests before going live



\### Test Approach

\- Manual testing first

\- Automated regression later (Playwright)

\- Positive and negative scenarios

\- Boundary value analysis for time slots and dates



\## 6. Test Environment



| Item | Details |

|------|---------|

| OS | Windows 11 |

| Browser | Chrome 125, Firefox 125, Edge 125 |

| Test URL | https://salon-staging.example.com |

| Database | MySQL 8 (test instance) |

| Tools | Postman, Jira, Git, Chrome DevTools |

| Test Data | Dummy users, dummy bookings |



\## 7. Entry Criteria

\- Requirements document approved

\- Test cases written and reviewed

\- Test environment ready

\- Test data prepared

\- Build deployed to staging



\## 8. Exit Criteria

\- All test cases executed

\- No critical or high severity bugs open

\- 95% pass rate achieved

\- Test summary report written

\- Stakeholder sign-off received



\## 9. Test Deliverables

\- Test Plan (this document)

\- Test Cases

\- Bug Reports

\- Test Summary Report

\- Test Metrics (pass/fail counts)



\## 10. Roles and Responsibilities



| Role | Person | Responsibility |

|------|--------|----------------|

| QA Engineer | Sujan Karki | Write test cases, execute tests, log bugs |

| Developer | Sujan Karki | Fix bugs, deploy builds |

| Product Owner | Salon Owner | Approve features, UAT |

| Scrum Master | Sujan Karki | Remove blockers, organize sprints |



\## 11. Schedule



| Phase | Duration |

|-------|----------|

| Test Planning | Day 1–2 |

| Test Case Writing | Day 3–5 |

| Environment Setup | Day 5 |

| Test Execution | Day 6–12 |

| Bug Fixing and Retesting | Day 10–14 |

| UAT | Day 15 |

| Test Closure | Day 16 |



\## 12. Risks and Mitigation



| Risk | Impact | Mitigation |

|------|--------|------------|

| Test environment not ready | Delays testing | Set up early |

| Bugs not fixed on time | Delays release | Daily bug review |

| Scope changes mid-sprint | Confusion | Freeze scope after planning |

| Limited time for regression | Missing bugs | Automate regression |

| Test data not realistic | Missing edge cases | Use realistic dummy data |



\## 13. Tools

\- Jira — bug tracking

\- Postman — API testing

\- Git and GitHub — version control

\- Chrome DevTools — debugging

\- MySQL Workbench — database validation

\- Playwright — automation (later phase)



\## 14. Approvals



| Role | Name | Signature | Date |

|------|------|-----------|------|

| QA Engineer | Sujan Karki | \_\_\_\_\_\_\_\_ | \_\_\_\_\_\_ |

| Product Owner | Salon Owner | \_\_\_\_\_\_\_\_ | \_\_\_\_\_\_ |

| Scrum Master | Sujan Karki | \_\_\_\_\_\_\_\_ | \_\_\_\_\_\_ |



\---



End of Test Plan

