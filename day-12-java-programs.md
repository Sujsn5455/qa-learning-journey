\# Day 12 — Arrays and ArrayList Java Programs



\## Program 1: Arrays



```java

public class Day12Arrays {

&#x20;   public static void main(String\[] args) {

&#x20;       String\[] testCases = {"Login", "Register", "Book", "Pay", "Logout"};

&#x20;       System.out.println("Total: " + testCases.length);

&#x20;       System.out.println("First: " + testCases\[0]);

&#x20;       System.out.println("Last: " + testCases\[testCases.length - 1]);



&#x20;       for (int i = 0; i < testCases.length; i++) {

&#x20;           System.out.println((i + 1) + ". " + testCases\[i]);

&#x20;       }

&#x20;   }

}

```



\### Output

Total: 5

First: Login

Last: Logout

1\. Login

2\. Register

3\. Book

4\. Pay

5\. Logout



\## Program 2: ArrayList



```java

import java.util.ArrayList;



public class Day12ArrayList {

&#x20;   public static void main(String\[] args) {

&#x20;       ArrayList<String> testCases = new ArrayList<>();

&#x20;       testCases.add("Login");

&#x20;       testCases.add("Register");

&#x20;       testCases.add("Book");



&#x20;       System.out.println("Total: " + testCases.size());

&#x20;       System.out.println("First: " + testCases.get(0));

&#x20;       System.out.println("Has Login? " + testCases.contains("Login"));



&#x20;       testCases.remove("Register");

&#x20;       System.out.println("After remove: " + testCases.size());

&#x20;   }

}

```



\### Output

Total: 3

First: Login

Has Login? true

After remove: 2



\## Program 3: Salon Test Data



```java

import java.util.ArrayList;



public class Day12SalonTestData {

&#x20;   public static void main(String\[] args) {

&#x20;       ArrayList<String> services = new ArrayList<>();

&#x20;       services.add("Haircut");

&#x20;       services.add("Facial");

&#x20;       services.add("Massage");



&#x20;       ArrayList<Integer> prices = new ArrayList<>();

&#x20;       prices.add(800);

&#x20;       prices.add(1500);

&#x20;       prices.add(2000);



&#x20;       int total = 0;

&#x20;       for (int i = 0; i < services.size(); i++) {

&#x20;           System.out.println(services.get(i) + " - Rs " + prices.get(i));

&#x20;           total += prices.get(i);

&#x20;       }

&#x20;       System.out.println("Total: Rs " + total);

&#x20;   }

}

```



\### Output

Haircut - Rs 800

Facial - Rs 1500

Massage - Rs 2000

Total: Rs 4300



\## What I Learned

\- Array declaration and access

\- ArrayList add, get, remove, size, contains

\- Looping with for and for-each

\- Real test data in ArrayList



\## Key Takeaway

Arrays hold fixed lists. ArrayList holds dynamic lists. Both are essential for QA automation.s

