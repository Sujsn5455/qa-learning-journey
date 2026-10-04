\# Day 12 — Arrays and ArrayList



\## Array (Fixed Size)

String\[] testCases = {"Login", "Register", "Book", "Pay"};

testCases\[0]      // Login

testCases.length  // 4



\## ArrayList (Dynamic Size)

import java.util.ArrayList;



ArrayList<String> testCases = new ArrayList<>();

testCases.add("Login");

testCases.add("Register");

testCases.get(0)   // Login

testCases.size()   // 2



\## ArrayList Common Methods

\- add(item) - Add item

\- get(index) - Get item

\- set(index, item) - Replace item

\- remove(index) - Remove at index

\- remove(item) - Remove by value

\- size() - Count items

\- contains(item) - Check exists

\- isEmpty() - Check empty

\- clear() - Remove all



\## Looping

for (int i = 0; i < testCases.size(); i++) {

&#x20;   System.out.println(testCases.get(i));

}



for (String testCase : testCases) {

&#x20;   System.out.println(testCase);

}



\## Array vs ArrayList

| Feature | Array | ArrayList |

|---------|-------|-----------|

| Size | Fixed | Dynamic |

| Length | arr.length | list.size() |

| Add | arr\[0] = "x" | list.add("x") |

| Import | No | java.util.ArrayList |



\## QA Applications

\- Store test cases

\- Store test data (users, bookings)

\- Iterate through tests

\- Compare expected vs actual results



\## Key Takeaway

Arrays hold fixed lists. ArrayList holds dynamic lists. Both are essential for automation.

