\# Day 11 — Control Flow Java Programs



\## Program 1: If-Else



```java

public class Day11IfElse {

&#x20;   public static void main(String\[] args) {

&#x20;       int total = 25;

&#x20;       int passed = 22;

&#x20;       double passRate = (passed \* 100.0) / total;



&#x20;       if (passRate >= 95) {

&#x20;           System.out.println("Release ready");

&#x20;       } else if (passRate >= 80) {

&#x20;           System.out.println("Needs minor fixes");

&#x20;       } else {

&#x20;           System.out.println("Needs major work");

&#x20;       }

&#x20;   }

}

```



\## Program 2: Switch



```java

public class Day11Switch {

&#x20;   public static void main(String\[] args) {

&#x20;       String\[] browsers = {"chrome", "firefox", "edge"};

&#x20;       for (String browser : browsers) {

&#x20;           switch (browser) {

&#x20;               case "chrome": System.out.println("Launching Chrome"); break;

&#x20;               case "firefox": System.out.println("Launching Firefox"); break;

&#x20;               default: System.out.println("Other browser");

&#x20;           }

&#x20;       }

&#x20;   }

}

```



\## Program 3: Loops



```java

public class Day11Loops {

&#x20;   public static void main(String\[] args) {

&#x20;       String\[] testCases = {"Login", "Register", "Book", "Pay"};

&#x20;       for (int i = 0; i < testCases.length; i++) {

&#x20;           System.out.println("Running: " + testCases\[i]);

&#x20;       }

&#x20;   }

}

```



\## Program 4: Salon Booking Check



```java

public class Day11SalonBookingCheck {

&#x20;   public static void main(String\[] args) {

&#x20;       String\[] bookings = {"BK\_001", "BK\_002", "BK\_003"};

&#x20;       String\[] statuses = {"Confirmed", "Pending", "Cancelled"};

&#x20;       int confirmed = 0;



&#x20;       for (int i = 0; i < bookings.length; i++) {

&#x20;           System.out.println(bookings\[i] + " -> " + statuses\[i]);

&#x20;           if (statuses\[i].equals("Confirmed")) confirmed++;

&#x20;       }



&#x20;       System.out.println("Confirmed bookings: " + confirmed);

&#x20;   }

}

```



\## What I Learned

\- if/else, switch, for, while, do-while

\- break and continue

\- Real QA example with Salon bookings



\## Key Takeaway

Control flow is the logic brain of test automation.

