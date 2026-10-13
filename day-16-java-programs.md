\# Day 16 — Exception Handling Java Programs



\## Program 1: Basic Exception Handling



```java

public class ExceptionDemo {

&#x20;   public static void main(String\[] args) {



&#x20;       try {

&#x20;           int result = 10 / 0;

&#x20;       } catch (ArithmeticException e) {

&#x20;           System.out.println("Caught: " + e.getMessage());

&#x20;       }



&#x20;       try {

&#x20;           System.out.println("Opening browser");

&#x20;           int x = 10 / 0;

&#x20;       } catch (ArithmeticException e) {

&#x20;           System.out.println("Error occurred");

&#x20;       } finally {

&#x20;           System.out.println("Closing browser (finally always runs)");

&#x20;       }



&#x20;       try {

&#x20;           String s = null;

&#x20;           System.out.println(s.length());

&#x20;       } catch (NullPointerException e) {

&#x20;           System.out.println("Null pointer caught");

&#x20;       }



&#x20;       System.out.println("Program continues after exceptions");

&#x20;   }

}

