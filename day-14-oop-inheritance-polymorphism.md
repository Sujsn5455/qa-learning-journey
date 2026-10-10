\# Day 14 — OOP: Inheritance and Polymorphism



\## Inheritance

A class can inherit fields and methods from another class.



```java

public class BaseTest {

&#x20;   public void openBrowser() {

&#x20;       System.out.println("Opening browser");

&#x20;   }

}



public class LoginTest extends BaseTest {

&#x20;   public void runLoginTest() {

&#x20;       System.out.println("Running login test");

&#x20;   }

}

