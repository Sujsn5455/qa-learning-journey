\# Day 16 — Exception Handling in Java



\## What is an Exception?

An unexpected event that disrupts normal program flow.



Examples:

\- Divide by zero

\- Array out of bounds

\- Null pointer

\- File not found

\- Element not found (automation)



\## try-catch

Wrap risky code in try. Handle errors in catch.



```java

try {

&#x20;   int result = 10 / 0;

} catch (ArithmeticException e) {

&#x20;   System.out.println("Error: " + e.getMessage());

}

