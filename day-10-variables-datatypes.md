\# Day 10 — Variables, Data Types, Operators



\## What is a Variable?

A named container that stores a value. The value can change.



\## Java Data Types



\### Primitive Types

| Type | Size | Example |

|------|------|---------|

| byte | 1 byte | 100 |

| short | 2 bytes | 1000 |

| int | 4 bytes | 25 |

| long | 8 bytes | 9000000L |

| float | 4 bytes | 3.14f |

| double | 8 bytes | 95.5 |

| char | 2 bytes | 'A' |

| boolean | 1 bit | true/false |



\### Reference Type

| Type | Example |

|------|---------|

| String | "Hello QA" |



\## Variable Naming Rules

\- Start with letter, $, or \_

\- Cannot start with number

\- Cannot be a Java keyword

\- Case-sensitive

\- Use camelCase: testCaseCount



\## Operators



\### Arithmetic

\+ - \* / %



\### Comparison

== != > < >= <=



\### Logical

\&\& || !



\### Assignment

= += -= \*= /=



\## Why This Matters for QA

\- Store test data

\- Track results

\- Calculate metrics

\- Compare expected vs actual



\## Key Takeaway

Variables store data. Data types define what kind of data. Operators manipulate data.



\# Day 10 — First Java Programs



\## Program 1: Test Report Variables



```java

public class Day10Variables {

&#x20;   public static void main(String\[] args) {

&#x20;       String testerName = "Sujan Karki";

&#x20;       String projectName = "Salon Booking System";

&#x20;       int totalTestCases = 25;

&#x20;       int passedTestCases = 22;

&#x20;       int failedTestCases = 3;

&#x20;       double passRate = 88.0;

&#x20;       boolean isReadyForRelease = false;



&#x20;       System.out.println("=== QA Test Report ===");

&#x20;       System.out.println("Tester: " + testerName);

&#x20;       System.out.println("Project: " + projectName);

&#x20;       System.out.println("Total Test Cases: " + totalTestCases);

&#x20;       System.out.println("Passed: " + passedTestCases);

&#x20;       System.out.println("Failed: " + failedTestCases);

&#x20;       System.out.println("Pass Rate: " + passRate + "%");

&#x20;       System.out.println("Ready for Release: " + isReadyForRelease);

&#x20;   }

}

