## Description

<div><p>Anton decided to get ready for an Olympiad in Informatics. Ilya prepared $n$ tasks for him to solve. It is possible to submit the solution for the $i$-th task in the first $d_{i}$ days only. Anton <span class="tex-font-style-bf">cannot</span> solve more than one task a day. Ilya estimated the usefulness of the $i$-th tasks as $r_{i}$ and divided the tasks into three topics, the topic of the $i$-th task is $type_{i}$.</p><p>Anton wants to solve exactly $a$ tasks on the first topic, $b$ tasks on the second topic and $c$ tasks on the third topic. Tell Anton if it is possible to do so, and if it is, calculate the maximum total usefulness of the tasks he may solve.</p></div><div class="input-specification"><p>The first line of input contains a single integer $t$ ($1 \le t \le 10^4$)&nbsp;— the number of test cases.</p><p>The first line of each test case contains four integers $n, a, b, c$ ($1 \le n \le 10^5$, $0 \le a, b, c \le n$).</p><p>The following $n$ lines contain three integers each&nbsp;— $r_i, type_i, d_i$ ($0 \le r_i \le 10^{9}$, $1 \le type_i \le 3$, $1 \le d_i \le n$).</p><p>The sum of $n$ over all test cases does not exceed $10^5$.</p></div><div class="output-specification"><p>For each test case print $-1$ if Anton cannot reach his goal; otherwise, print the maximum usefulness of the tasks he will solve.</p></div>

## Input

<p>The first line of input contains a single integer $t$ ($1 \le t \le 10^4$)&nbsp;— the number of test cases.</p><p>The first line of each test case contains four integers $n, a, b, c$ ($1 \le n \le 10^5$, $0 \le a, b, c \le n$).</p><p>The following $n$ lines contain three integers each&nbsp;— $r_i, type_i, d_i$ ($0 \le r_i \le 10^{9}$, $1 \le type_i \le 3$, $1 \le d_i \le n$).</p><p>The sum of $n$ over all test cases does not exceed $10^5$.</p>

## Output

<p>For each test case print $-1$ if Anton cannot reach his goal; otherwise, print the maximum usefulness of the tasks he will solve.</p>





```input1|2,3,4,5,6,11,12,13,14,15
4
4 1 1 0
1 2 1
1 1 1
0 1 2
1 2 2
3 1 1 1
1 1 2
7 2 1
9 3 2
4 2 1 0
100 2 1
5 2 3
7 1 2
5 1 2
5 1 1 1
10 3 1
9 2 3
20 1 1
16 1 4
1 3 4
```




```output1
2
-1
17
35
```



## Note

<p>In the first test case from the sample test Anton can solve tasks $2$ and $4$.</p><p>In the second test case from the sample test it is impossible to fulfill Anton's wish.</p><p>In the third test case from the sample test it is optimal to solve tasks $2$, $3$ and $4$.</p><p>In the last test case from the sample test it is optimal to solve tasks $1$, $2$ and $4$.</p>
