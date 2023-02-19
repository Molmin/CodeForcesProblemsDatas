## Description

<div><p>Given an array $a$ of length $n$ and an integer $k$, find the number of indices $1 \leq i \leq n - k$ such that the subarray $[a_i, \dots, a_{i+k}]$ with length $k+1$ (<span class="tex-font-style-bf">not</span> with length $k$) has the following property: </p><ul> <li> If you multiply the first element by $2^0$, the second element by $2^1$, ..., and the ($k+1$)-st element by $2^k$, then this subarray is sorted in strictly increasing order. </li></ul> More formally, count the number of indices $1 \leq i \leq n - k$ such that $$2^0 \cdot a_i &lt; 2^1 \cdot a_{i+1} &lt; 2^2 \cdot a_{i+2} &lt; \dots &lt; 2^k \cdot a_{i+k}.$$ </div><div class="input-specification"><p>The first line contains an integer $t$ ($1 \leq t \leq 1000$)&nbsp;— the number of test cases.</p><p>The first line of each test case contains two integers $n$, $k$ ($3 \leq n \leq 2 \cdot 10^5$, $1 \leq k &lt; n$)&nbsp;— the length of the array and the number of inequalities.</p><p>The second line of each test case contains $n$ integers $a_1, a_2, \dots, a_n$ ($1 \leq a_i \leq 10^9$)&nbsp;— the elements of the array.</p><p>The sum of $n$ across all test cases does not exceed $2 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, output a single integer&nbsp;— the number of indices satisfying the condition in the statement.</p></div>

## Input

<p>The first line contains an integer $t$ ($1 \leq t \leq 1000$)&nbsp;— the number of test cases.</p><p>The first line of each test case contains two integers $n$, $k$ ($3 \leq n \leq 2 \cdot 10^5$, $1 \leq k &lt; n$)&nbsp;— the length of the array and the number of inequalities.</p><p>The second line of each test case contains $n$ integers $a_1, a_2, \dots, a_n$ ($1 \leq a_i \leq 10^9$)&nbsp;— the elements of the array.</p><p>The sum of $n$ across all test cases does not exceed $2 \cdot 10^5$.</p>

## Output

<p>For each test case, output a single integer&nbsp;— the number of indices satisfying the condition in the statement.</p>





```input1
6
4 2
20 22 19 84
5 1
9 5 3 2 1
5 2
9 5 3 2 1
7 2
22 12 16 4 3 22 12
7 3
22 12 16 4 3 22 12
9 3
3 9 12 3 9 12 3 9 12
```




```output1
2
3
2
3
1
0
```



## Note

<p>In the first test case, both subarrays satisfy the condition: </p><ul> <li> $i=1$: the subarray $[a_1,a_2,a_3] = [20,22,19]$, and $1 \cdot 20 &lt; 2 \cdot 22 &lt; 4 \cdot 19$. </li><li> $i=2$: the subarray $[a_2,a_3,a_4] = [22,19,84]$, and $1 \cdot 22 &lt; 2 \cdot 19 &lt; 4 \cdot 84$. </li></ul> In the second test case, three subarrays satisfy the condition: <ul> <li> $i=1$: the subarray $[a_1,a_2] = [9,5]$, and $1 \cdot 9 &lt; 2 \cdot 5$. </li><li> $i=2$: the subarray $[a_2,a_3] = [5,3]$, and $1 \cdot 5 &lt; 2 \cdot 3$. </li><li> $i=3$: the subarray $[a_3,a_4] = [3,2]$, and $1 \cdot 3 &lt; 2 \cdot 2$. </li><li> $i=4$: the subarray $[a_4,a_5] = [2,1]$, but $1 \cdot 2 = 2 \cdot 1$, so this subarray doesn't satisfy the condition. </li></ul>
