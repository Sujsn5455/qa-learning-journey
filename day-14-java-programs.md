

Paste this content:



````markdown

\# Day 14 — Inheritance and Polymorphism Java Programs



\## Program 1: Inheritance



```java

public class BaseTest {

&#x20;   public void openBrowser() {

&#x20;       System.out.println("Opening Chrome browser");

&#x20;   }

&#x20;   public void closeBrowser() {

&#x20;       System.out.println("Closing browser");

&#x20;   }

&#x20;   public void setup() {

&#x20;       System.out.println("Base setup");

&#x20;   }

}



public class LoginTest extends BaseTest {

&#x20;   public void runLoginTest() {

&#x20;       System.out.println("Running login test");

&#x20;   }

&#x20;   @Override

&#x20;   public void setup() {

&#x20;       System.out.println("Login test setup - opening login page");

&#x20;   }

}



public class InheritanceDemo {

&#x20;   public static void main(String\[] args) {

&#x20;       LoginTest test = new LoginTest();

&#x20;       test.openBrowser();

&#x20;       test.setup();

&#x20;       test.runLoginTest();

&#x20;       test.closeBrowser();

&#x20;   }

}

