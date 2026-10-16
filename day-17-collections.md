\# Day 17 — Java Collections: List, Set, Map



\## What is the Collections Framework?

A set of classes and interfaces for storing groups of objects.



\## Three Main Interfaces



| Interface | Order | Duplicates |

|-----------|-------|------------|

| List | Yes | Yes |

| Set | No | No |

| Map | No | Keys unique |



\## List — ArrayList



```java

List<String> testCases = new ArrayList<>();

testCases.add("Login");

testCases.add("Register");

testCases.add("Login");   // duplicate allowed

System.out.println(testCases.get(0));

System.out.println(testCases.size());

