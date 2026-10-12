s# Day 15 — Encapsulation and Abstraction Java Programs



\## Program 1: Encapsulation



```java

public class TestCase {

&#x20;   private String name;

&#x20;   private String status;



&#x20;   public TestCase(String name, String status) {

&#x20;       this.name = name;

&#x20;       this.status = status;

&#x20;   }



&#x20;   public String getName() { return name; }

&#x20;   public void setName(String name) { this.name = name; }



&#x20;   public String getStatus() { return status; }

&#x20;   public void setStatus(String status) {

&#x20;       if (status.equals("Passed") || status.equals("Failed") || status.equals("Blocked")) {

&#x20;           this.status = status;

&#x20;       } else {

&#x20;           System.out.println("Invalid status: " + status);

&#x20;       }

&#x20;   }

}



public class EncapsulationDemo {

&#x20;   public static void main(String\[] args) {

&#x20;       TestCase tc = new TestCase("Login Test", "Passed");

&#x20;       System.out.println("Name: " + tc.getName());

&#x20;       System.out.println("Status: " + tc.getStatus());



&#x20;       tc.setStatus("Failed");

&#x20;       System.out.println("Updated: " + tc.getStatus());



&#x20;       tc.setStatus("Whatever");

&#x20;       System.out.println("Still: " + tc.getStatus());

&#x20;   }

}

