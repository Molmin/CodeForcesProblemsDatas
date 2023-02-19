## Description

<div><p>In the work of a doctor, it is important to maintain the anonymity of clients and the results of tests. The test results are sent to everyone personally by email, but people are very impatient and they want to know the results right away.</p><p>That's why in the testing lab "De-vitro" doctors came up with an experimental way to report the results. Let's assume that $n$ people took the tests in the order of the queue. Then the chief doctor Sam can make several statements, in each telling if there is a sick person among the people in the queue from $l$-th to $r$-th (inclusive), for some values $l$ and $r$.</p><p>During the process, Sam will check how well this scheme works and will be interested in whether it is possible to find out the test result of $i$-th person from the information he announced. And if it can be done, then is that patient sick or not.</p><p>Help Sam to test his scheme.</p></div><div class="input-specification"><p>The first line contains two integers $n$, $q$ ($1 \le n, q \le 2 \cdot 10^5$) — the number of people and the number of queries.</p><p>In each of the next $q$ lines, the description of the query is given. The first number in the line is $t$ ($t = 0$ or $t = 1$) — the type of the query.</p><p>If $t = 0$, the line contains three more integers $l, r, x$ ($1 \le l \le r \le n$, $x = 0$ or $x = 1$). This query means that Sam tells that among the people in the queue from $l$-th to $r$-th (inclusive): </p><ul> <li> there was at least one sick person, if $x=1$, </li><li> there is no sick people, if $x=0$. </li></ul><p>If $t = 1$, the line contains one more integer $j$ ($1 \le j \le n$) — the position of the patient in the queue, for which Sam wants to know the status.</p><p>All queries are correct, that means that there always exists an example of the queue of length $n$ for which all reported results (statements from queries with $t = 0$) are true.</p></div><div class="output-specification"><p>After each Sam question (query with $t = 1$) print:</p><ul> <li> "<span class="tex-font-style-tt">NO</span>", if the patient is definitely not sick, </li><li> "<span class="tex-font-style-tt">YES</span>", if the patient is definitely sick. </li><li> "<span class="tex-font-style-tt">N/A</span>", if it is impossible to definitely identify the status of patient having the given information. </li></ul></div>

## Input

<p>The first line contains two integers $n$, $q$ ($1 \le n, q \le 2 \cdot 10^5$) — the number of people and the number of queries.</p><p>In each of the next $q$ lines, the description of the query is given. The first number in the line is $t$ ($t = 0$ or $t = 1$) — the type of the query.</p><p>If $t = 0$, the line contains three more integers $l, r, x$ ($1 \le l \le r \le n$, $x = 0$ or $x = 1$). This query means that Sam tells that among the people in the queue from $l$-th to $r$-th (inclusive): </p><ul> <li> there was at least one sick person, if $x=1$, </li><li> there is no sick people, if $x=0$. </li></ul><p>If $t = 1$, the line contains one more integer $j$ ($1 \le j \le n$) — the position of the patient in the queue, for which Sam wants to know the status.</p><p>All queries are correct, that means that there always exists an example of the queue of length $n$ for which all reported results (statements from queries with $t = 0$) are true.</p>

## Output

<p>After each Sam question (query with $t = 1$) print:</p><ul> <li> "<span class="tex-font-style-tt">NO</span>", if the patient is definitely not sick, </li><li> "<span class="tex-font-style-tt">YES</span>", if the patient is definitely sick. </li><li> "<span class="tex-font-style-tt">N/A</span>", if it is impossible to definitely identify the status of patient having the given information. </li></ul>





```input1
6 9
0 4 5 0
1 5
1 6
0 4 6 1
1 6
0 2 5 1
0 2 2 0
1 3
1 2
```




```output1
NO
N/A
YES
YES
NO
```



## Note

<p>In the first test for the five first queries:</p><ol> <li> Initially Sam tells that people $4$, $5$ are not sick. </li><li> In the next query Sam asks the status of the patient $5$. From the previous query, we know that the patient is definitely not sick. </li><li> In the next query Sam asks the status of the patient $6$. We don't know any information about that patient now. </li><li> After that Sam tells that there exists a sick patient among $4$, $5$, $6$. </li><li> In the next query Sam asks the status of the patient $6$. Now we can tell that this patient is definitely sick. </li></ol>
