\# Salon Booking System — Test Cases



\## Module: Login



\### TC\_001 — Login with valid credentials



\- Preconditions: User is registered and app is open

\- Test Steps:

&#x20; 1. Enter valid email in email field

&#x20; 2. Enter valid password in password field

&#x20; 3. Click Login button

\- Test Data: email: sujan@test.com, password: Test@123

\- Expected Result: User is redirected to dashboard

\- Actual Result: Not executed

\- Status: Not Run

\- Priority: High



\### TC\_002 — Login with wrong password



\- Preconditions: User is registered

\- Test Steps:

&#x20; 1. Enter valid email

&#x20; 2. Enter wrong password

&#x20; 3. Click Login button

\- Test Data: email: sujan@test.com, password: WrongPass

\- Expected Result: Error message "Invalid credentials" is shown

\- Actual Result: Not executed

\- Status: Not Run

\- Priority: High

