\# Day 13 — OOP: Class, Object, Constructor



\## What is OOP?

Object-Oriented Programming organizes code into objects that contain data and behavior.



\## 1. Class



A class is a blueprint for creating objects. It defines what fields and methods an object will have.



```java

public class TestCase {

&#x20;   String name;

&#x20;   String status;

&#x20;   int priority;

}





2\. Object

An object is an instance of a class. You create it with the new keyword.



java

TestCase tc1 = new TestCase();

tc1.name = "Login Test";

tc1.status = "Passed";

tc1.priority = 1;

Explanation:



new TestCase() — creates a new object



tc1 — variable that holds the object



tc1.name — access the name field



You can create many objects from one class



3\. Constructor

A special method that runs automatically when an object is created.



java

public TestCase(String name, String status, int priority) {

&#x20;   this.name = name;

&#x20;   this.status = status;

&#x20;   this.priority = priority;

}





Explanation:



Same name as the class



No return type



Runs when new TestCase(...) is called



Sets initial values for the object



4\. this keyword

this refers to the current object. Used when parameter names match field names.



java

public TestCase(String name) {

&#x20;   this.name = name;   // this.name = field, name = parameter

}

Types of Constructors

Default Constructor

No parameters. Java provides one if you do not write any.



java

public TestCase() {

}

Parameterized Constructor

Takes parameters to set initial values.



java

public TestCase(String name, String status) {

&#x20;   this.name = name;

&#x20;   this.status = status;

}

