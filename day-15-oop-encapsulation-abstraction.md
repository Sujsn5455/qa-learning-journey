\# Day 15 — OOP: Encapsulation and Abstraction



\## Encapsulation

Hiding data and allowing access only through methods.



```java

public class TestCase {

&#x20;   private String name;

&#x20;   private String status;



&#x20;   public String getName() { return name; }

&#x20;   public void setName(String name) { this.name = name; }



&#x20;   public String getStatus() { return status; }

&#x20;   public void setStatus(String status) { this.status = status; }

}

