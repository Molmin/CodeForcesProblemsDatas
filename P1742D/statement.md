## Description

<div><p>Given an array of $n$ positive integers $a_1, a_2, \dots, a_n$ ($1 \le a_i \le 1000$). Find the maximum value of $i + j$ such that $a_i$ and $a_j$ are coprime,$^{\dagger}$ or $-1$ if no such $i$, $j$ exist.</p><p>For example consider the array $[1, 3, 5, 2, 4, 7, 7]$. The maximum value of $i + j$ that can be obtained is $5 + 7$, since $a_5 = 4$ and $a_7 = 7$ are coprime.</p><p>$^{\dagger}$ Two integers $p$ and $q$ are <a href="https://en.wikipedia.org/wiki/Coprime_integers">coprime</a> if the only positive integer that is a divisor of both of them is $1$ (that is, their <a href="https://en.wikipedia.org/wiki/Greatest_common_divisor">greatest common divisor</a> is $1$).</p></div><div class="input-specification"><p>The input consists of multiple test cases. The first line contains an integer $t$ ($1 \leq t \leq 10$)&nbsp;— the number of test cases. The description of the test cases follows.</p><p>The first line of each test case contains an integer $n$ ($2 \leq n \leq 2\cdot10^5$)&nbsp;— the length of the array.</p><p>The following line contains $n$ space-separated positive integers $a_1$, $a_2$,..., $a_n$ ($1 \leq a_i \leq 1000$)&nbsp;— the elements of the array.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2\cdot10^5$.</p></div><div class="output-specification"><p>For each test case, output a single integer &nbsp;— the maximum value of $i + j$ such that $i$ and $j$ satisfy the condition that $a_i$ and $a_j$ are coprime, or output $-1$ in case no $i$, $j$ satisfy the condition.</p></div>

## Input

<p>The input consists of multiple test cases. The first line contains an integer $t$ ($1 \leq t \leq 10$)&nbsp;— the number of test cases. The description of the test cases follows.</p><p>The first line of each test case contains an integer $n$ ($2 \leq n \leq 2\cdot10^5$)&nbsp;— the length of the array.</p><p>The following line contains $n$ space-separated positive integers $a_1$, $a_2$,..., $a_n$ ($1 \leq a_i \leq 1000$)&nbsp;— the elements of the array.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2\cdot10^5$.</p>

## Output

<p>For each test case, output a single integer &nbsp;— the maximum value of $i + j$ such that $i$ and $j$ satisfy the condition that $a_i$ and $a_j$ are coprime, or output $-1$ in case no $i$, $j$ satisfy the condition.</p>





```input1|2,3,6,7,10,11
6
3
3 2 1
7
1 3 5 2 4 7 7
5
1 2 3 4 5
3
2 2 4
6
5 4 3 15 12 16
5
1 2 2 3 6
```




```output1
6
12
9
-1
10
7
```



## Note

<p>For the first test case, we can choose $i = j = 3$, with sum of indices equal to $6$, since $1$ and $1$ are coprime.</p><p>For the second test case, we can choose $i = 7$ and $j = 5$, with sum of indices equal to $7 + 5 = 12$, since $7$ and $4$ are coprime.</p>
